# tlz-selfbot
a simple selfbot for discord
- support [discord](http://dsc.gg/tlz)
## How to use
- rename the config.js.example to config.js, there's guide in the file
- install [this](https://github.com/Kyou-Izumi/advanced-discord-owo-tool-farm) then open cmd, npm start to make the config, cmd again and npm start then choose the account -> export config, copy the [yourname].json to the selfbot folder, change the owo section in config.json

## Edit website?
you can edit whatever you want the 
```batch
cd web
npm run build
```

## How to get token?
```js
window.webpackChunkdiscord_app.push([
	[Symbol()],
	{},
	req => {
		if (!req.c) return;
		for (let m of Object.values(req.c)) {
			try {
				if (!m.exports || m.exports === window) continue;
				if (m.exports?.getToken) return copy(m.exports.getToken());
				for (let ex in m.exports) {
					if (m.exports?.[ex]?.getToken && m.exports[ex][Symbol.toStringTag] !== 'IntlMessagesProxy') return copy(m.exports[ex].getToken());
				}
			} catch {}
		}
	},
]);

window.webpackChunkdiscord_app.pop();
console.log('%cWorked!', 'font-size: 50px');
console.log(`%cYou now have your token in the clipboard!`, 'font-size: 16px');
``` 
this script from [here](https://github.com/aiko-chan-ai/discord.js-selfbot-v13/)

### You can give me idea via 
discord: @tuilazerotwo | telegram: @tlzitsme
### Shout out
- advanced discord owo autofarm, [here](https://github.com/Kyou-Izumi/advanced-discord-owo-tool-farm/)</p>
- a big thanks to xFrogly for the bot base , [here](https://github.com/xFrogly/Discord-SelfBot)</p>
