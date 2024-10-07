[0-9] - Corresponda a qualquer dígito que esteja no intervalo de 0 a 9.
Ex.: 958 = 3 matches (9, 5, 8)

\d - Shorthand, corresponda a qualquer dígito que esteja no intervalo de 0 a 9.
Ex.: 958 = 3 matches (9, 5, 8)

\D - Corresponda a qualquer caractere que não seja um dígito (0-9).
Ex.: 1s2d = 2 matches (s, d)

. - Corresponda a qualquer caractere (exceto quebra de linha (U+000A))

## Grupo de captura
Para criar um grupo de captura, coloque um \d entre parênteses para inseri-lo em um grupo e depois coloque um \1 para fazer uma referência àquilo que foi anteriormente capturado.
(\d)\d\1
- (\d) - Corresponde ao primeiro dígito e o captura
- \d - Corresponde ao próximo dígito, mas o captura, pque não está entre parênteses
- \1 referenci o dígito capturado


## Quantificadores
Ex.: \d{3}-?\d{3}-?\d{4}
- O número entre chaves representa quantas ocorrências desses dígitos você quer que ele procure.
- O ponto de interrogação indica que o caractere é opcional (pode haver zero ou uma ocorrência)
