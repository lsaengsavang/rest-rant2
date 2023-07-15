# Project REST-Rant

REST-Rant is an app where users can review restaurants.

## Routes

| Method | Path                       | Purpose                                          |
| ------ | -------------------------- | ------------------------------------------------ |
| GET    | `/`                        | Home page                                        |
| GET    | `/places`                  | Places index page                                |
| POST   | `/places`                  | Create a new place                               |
| GET    | `/places/new`              | New form for a place                             |
| GET    | `/places/:id`              | Details about a particular place                 |
| PUT    | `/places/:id`              | Update a particular place                        |
| GET    | `/places/:id/edit`         | Edit form for a place                            |
| DELETE | `/places/:id`              | Delete a particular place                        |
| POST   | `/places/:id/rant`         | Create a rant (comment) about a particular place |
| DELETE | `/places/:id/rant/:rantId` | Delete a rant (comment) about a particular place |
| GET    | `*`                        | 404 page (matches any route not defined above)   |

**places**

| Field    | Type   |
| -------- | ------ |
| name     | String |
| city     | String |
| state    | String |
| cuisines | String |
| pic      | String |