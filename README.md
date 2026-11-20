# ConnectFilter

ConnectFilter is a local Chrome extension for reviewing and managing LinkedIn connection requests using keyword and mutual-connection filters.

It always starts with a preview, requires confirmation before accepting requests, and limits each run to 25 actions.

> ConnectFilter is an independent project and is not affiliated with, endorsed by, or sponsored by LinkedIn. Use it in accordance with LinkedIn's terms and your own judgment.

## Features

- Preview matching requests before taking action
- Match keywords from the request card (for example, `founder`, `VC`, or `angel`)
- Set a minimum number of mutual connections
- Pace actions with randomized 2–6 second delays
- Cap both accepts and ignores at 25 actions per session
- Keep filter preferences in local browser storage only

## Install

1. Clone or download this repository.
2. Open `chrome://extensions` in Chrome or another Chromium-based browser.
3. Enable **Developer mode**.
4. Select **Load unpacked** and choose this project folder.
5. Open LinkedIn's received invitations page.
6. Click the ConnectFilter icon and select **Preview matches first**.

## Usage

1. Enter comma-separated keywords and/or set a mutual-connection minimum.
2. Select **Preview matches first** and review every match.
3. Select **Accept** to proceed with the previewed filter, or **Ignore visible** to decline only the requests currently visible in LinkedIn.
4. Keep the LinkedIn tab open until the action finishes.

## Privacy

ConnectFilter runs entirely in your browser. It reads the invitation cards on LinkedIn's invitation-manager page only, and stores your keyword and mutual-connection preferences locally through Chrome storage. It does not send your request data to a server.

## Development

This is a Manifest V3 extension with no build step. After changing the source, return to `chrome://extensions` and select the reload button on the ConnectFilter card.

## License

[MIT](LICENSE)
