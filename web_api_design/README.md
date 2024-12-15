## Web API Design - Crafting Interfaces that Developers Love
### Brian Mulloy

#### Nouns are good; verbs are bad

- Use two base URLs per resource
- Keep verbs out of your base URLs
- Use HTTP verbs to operate on the collections and elements

Ex.: 

| URL/Resource | POST           | GET       | PUT              | DELETE          |
| ------------ | -------------- | --------- | ---------------- | --------------- |
| /dogs        | Create new dog | List dogs | Bulk update dogs | Delete all dogs |
| /dogs/1234   | Error          | Show dog  | If exist update  | Delete dog      |

#### Plural nouns and concrete names

Should you choose singular or plural nouns for your resource names? Popular
APIs use both.

Above all, avoid a mixed model in which you use singular for some resources, plural for others.

In summary, an intuitive API uses plural rather than singular nouns, and concrete rather than abstract names.
