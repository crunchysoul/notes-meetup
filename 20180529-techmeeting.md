# Redux Sage: Andrew
- Redux Saga
- Redux saga manage side effect
- background process -> saga
- Es6, `generator`, pure functional
- `yield` control the execution of generator `.next()`
- React Layers: React::view -> Redux::state -> Redux sage::side effects

## code:
```javascript
// sage in one place for the module
export default rootSaga;

//side effect wait for action being dispatched
yield take(foo)
```

## Flow Common pattern:

### Flow Sagas:
- one features
- trigger by actions
-
### Common Sagas:
- always returning
- error management for the flow saga

## Signal Message pattern:
input & output saga

## Retro
- saga waiting for trigger
- action creator pure
- testing for business idea

# GraphQL api Elixir Absinthe: Tom
- json vs graphQL
- one endpoint, graphql documents what clients want
- three types of docs:
  - queries (can choose field)
  - mutations (change POST DELETE.)
  - Subscriptions (listening, websocket, hook, long socket)

# Queries
- specify exactly field and relationship you need
- as deep as schema allowed
- json is about balance what to include
- graphql can be flexible
```json

```

```elixir
forward to schema
Resolvers/3(parent, params, //tomdunno)
field return field takes args params
paramtise query make a funciton from query
query variables
query getTribeByID create by client
```

- get doc and schema for free from absinthe
- absinthe with phx, standalone

# Mutations
- make changes
- tailor the field and resp

```elixir
mutatio do
field: create_story, :story_result do
arg :input, non_null
end
```
```json
mutation {
createStory({

    }){
  __typename
  error
  }
}
```
- restful return http error
- graphql return error resp
- Revolver

# Subscriptions
- submit doc that get executed later
- think uber auto update car location

```elixir
subscription
config(topic, input)
trigger
"*" global channel
```

# More
- interfaces
- Unions: search OR
- Auth
- Middleware, error format
- Data loader solve n+1, pre-fetching! preload

# Tools
- GraphQl
- Client libs apollo, relay
- graphql voyager
- awesome graphql

# Publication you api using graphQL
- graphql is good for latency, optimal, cruel for database
- cache too flexible to caching
- tool to find all most frequent path for caching
- graphcms.com
- schema to cms
- graphql schema is better
 
# api
url -> here is the things -> grab things

# Art exhibition backend api
