
如果在 remote JS debugging 环境下运行正常, 但是在 release 环境中会出现问题的话，去考虑一下 js 兼容性的问题。

因为在 debugging 时 js 运行环境为 chrome v8，
但是在 release 时，是基于 react-native 内置的环境。
