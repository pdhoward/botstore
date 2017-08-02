
## BotStore App

The worlds greatest collection of bots for sale or lease

## Getting Set Up

Getting the app running on your local machine takes only a few steps:

1. clone the project - `git clone https://github.com/pdhoward/botstore.git
2. install its dependencies - `npm install`
3. start the app - npm run start

## Backend Server

Note that a backend server is used strictly for testing

The set of methods for all required operations

### `getAll()`
* Returns a Promise which resolves to a JSON object containing a collection of bot objects.
* This collection represents the bots currently available in the store

### `order(bot, customer)`
* bot: `<Object>` containing at minimum an `id` attribute
* customer: `<String>` contains customer id  
* Returns a Promise which resolves to a JSON object containing the response data of the POST request

### `search(query, maxResults)`
* query: `<String>` containing bot name or description
* maxResults: `<Integer>` Cap on search results
* Returns a Promise which resolves to a JSON object containing a collection of bot objects.
* These bots are not interactive (at this stage). Returns raw search results only. IN the future, we expect that bots would be active in selling themselves, demonstrating the interactive brand concept pioneered by xio

## License and Use
 [LICENSE](LICENSE.txt).

## Triggers
The web store is augmented with a suite of microservices enabling this store for a messaging world. The set of trigger words represent the set of actions which are mapped to microservices (other bots) for helping a customer navigate search and complete a transactions
[TRIGGER_WORDS](TRIGGER_WORDS.md).
That list of trigger words are provided to help you better explore the messaging demonstration for chaoticbots

Note that the chaotic platforms employ natural language processing (NLP) and  other AI techiques and technologies to facilitate brand interactions

## Contributing

For details, check out [CONTRIBUTING](CONTRIBUTING.md).
xio labs and affiliates
connecting businesses with the conversational economy
