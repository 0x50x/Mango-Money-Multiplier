it's a funding arbitrage bot for mangomarkets



1. install docker and docker-compose
2. sudo docker-compose up 
3. wait
4. you need your private key as machine readable in the root as id.json
5. if you need to translate your private key to uint8, plz check the bs58 npmjs packagae.
6. it's probably easier for you to download and installs solana cli and run solana-keygen new, then copypasta your id.json from ~/.config/solana/id.json
7. this is actually designed to trade for people that delegate to you via mango, so right now all your addresses you'd want to trade are defined here. change these pubkeys.

./mango-service-v3/src/mango.simple.client.ts:let meAndThePeeps = ["5sBpMQgTi7phxqRnErfbwx29vUsbUZoy1MLgY7aXuqeo", "GvSCxCi3y2Mt4JPExhLEZXTbYVGBXv9DNXYomvwRVEak"]

8. sudo docker build . or sudo docker-compose --build
9. great, it's running?
10. cd py && curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python - && source ~/.poetry/env
11. pip install tenacity httpx pydantic 
12. python example3_market_maker.py
13. I accept both tips stacc.sol and PRs


## Important

1. Risk only what you can afford to lose.
2. Trading at leverage is extremely risky, and there is a chance you may lose all your funds.
3. In no way do I or any other party imply let alone assure results.
4. Historical data is no indication of future activity.
5. This is extremely alpha software, largely undocumented and completely without tests or helpful comments. Use at your own risk.
6. Nothing I do or say should ever be misconstrued as financial advice.

## Back to your scheduled programming...

I forgot you need to do this: mango-client-v3$ ts-node examples/example.ts  it expects your id.json in the default solana dir


Finally sat down and had time to work thru kinks, this has been running a few hours - gonna leave this here and update after a nap probably :)

![image](https://user-images.githubusercontent.com/22843601/160265506-eac8aefb-07b8-44e4-8fe1-1a7f23295da8.png)


oops aged well :)

![image](https://user-images.githubusercontent.com/22843601/160292441-5d63ba6c-4808-4d0c-8653-ef0c1b23a1d6.png)

