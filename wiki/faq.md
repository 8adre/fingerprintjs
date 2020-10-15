# FAQ

#### Can I use this library to uniquely identify users?

No, you cannot. This library is built to be able to associate string identifiers with devices. Since there are a lot of identical devices, you will get a lot of identical identifiers.

#### OK, I get it, I cannot _uniquely_ identify users, but can I identify users at all?

No, you cannot. This library is strictly for non-deterministic device identification.

#### How good is your library? Can you guarantee that different devices will have different identifiers?

This library is not good. It has an error margin of 20-50% (better on desktops, worse on iPhones)

#### Can you improve the library to be 100% accurate for device identification?

I don't think it is possible now and don't think it will be possible in the future.

#### Can you improve the library to be more accurate (since you cannot make it 100% accurate)?

This is not the goal of this library, for better results, please use the PRO version: https://fingerprintjs.com

#### How can I build a complete identification solution?

You should use our commercial "PRO" version: https://fingerprintjs.com

#### The fingerprint is changing frequently for me, is the library broken?

Well, most likely not. You may have different user agents (because of the browser upgrades), or different screen resolutions. You can disable corresponding options (please see README and Wiki for details). The library provides a callback/extension system that for example allows you to use UserAgent parsers and cut off the frequently changing parts of user agents (such as version numbers). If you're sure it is a bug, please submit an issue and don't forget to attach the relevant info about which component, participating in fingerprint building, changes for your from call to call.