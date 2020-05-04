# Changes

Here is the list of all changes from official app.

## Current changes

* Mention user by its name instead of username: right click on mention suggestion.
* Option "Nobody" in profile photo privacy settings.
* Links and usernames in user bios are now clickable.
* Copy bot button callback data by right clicking on it.
* Increased size of caption field to 150px (\~5 lines).
* Show and hide pinned message from chat menu.
* Show linked dicussion group/channel in profile.
* Always show edit timer.
* "About" box link in drawer moved to app name to increase space for version.
* Options "Show custom settings" and "Restart Kotatogram" in three-dots settings' menu.
* JSON translations to rewrite phrases that are not in official. Russian included in app.
* Admin ranks now shown in member list.
* Fixed "Channel is not accessible" error, when trying to open discussion channel from group post if target channel is private and you are not subscribed to it.
* Changed "members" to "subscribers" for channels.
* Keyboard shortcut to save draft to cloud (Ctrl+S by default).
* Collapsed archived chats now have an icon.
* JSON-configured options. You have to restart app to see changes.
  * `fonts` - app font repacling.
    * `main` - replace main font.
    * `semibold` - replace semibold font.
    * `semibold_is_bold` - should semibold font be set to bold or not.
    * `monospaced` - replace monospaced font.
  * `sticker_height` - sticker height in chat (from 128 to 256).
  * `big_emoji_outline` - enable/disable white outline for big emoji.
  * `always_show_scheduled` - show scheduled messages button always or only when there are scheduled messages.
  * `show_chat_id` - show chat id in profile.
  * `net_speed_boost` - increased download/upload speed.<br>**Warning!** If you have low connection speed, better not to touch this option. More info: https://github.com/telegramdesktop/tdesktop/pull/6442#issuecomment-525663010<br>Available values:
  	* `null` or `0` - default speed (like in official client).
  	* `"low"` or `1`
  	* `"medium"` or `2`
  	* `"high"` or `3` - fastest speed, like in [TDMT](https://github.com/mediatube/tdesktop).
  * `show_phone_in_drawer` - hides phone number in drawer when set to `false`.
  * `scales` - custom scales in settings. Maximum 6 scales from 75-300 allowed.


## Was made into official app
* Allow scales below 100 to be saved in local settings.
* Resize photo message when there are additional texts (author name or caption).
* Show restriction date to user.

## Deprecated
* Font changing start options `-mainfont`, `-semiboldfont`, `-semiboldisbold`, `-monospacefont`.