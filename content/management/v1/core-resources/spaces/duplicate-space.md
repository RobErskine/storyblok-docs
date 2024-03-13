---
title: Duplicate a Space
---

Duplicate a space and all it's content entries and components; Assets will not be duplicated and still will reference the original space.

| Property | Description |
|---|---|
| `space[name]` | Name of your space; **required** |
| `space[domain]` | Domain for your default preview url |
| `space[story_published_hook]` | Published Webhook URL |
| `space[searchblok_id]` | Searchblok id, if available |
| `space[environments]` | Array of `name` and `location` (url) objects |
| `dup_id` | The numeric id of the original space |
| `assign_partner` | Boolean. Whether to create this new space in your partner space, if you are part of one |

;examplearea

Example Request

<RequestExample url="https://mapi.storyblok.com/v1/spaces/" httpMethod="POST" :requestObject='{"dup_id":12422, "space":{"name":"Example Space"}}'></RequestExample>

You will receive a [space object](#core-resources/spaces/the-space-object) as response.
