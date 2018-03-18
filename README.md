# MP Mini Delta Web

## Updating the factory web UI

1. Download and unzip `MP-Mini-Delta-Web` from GitHub.
2. Point a web browser window to your printer's IP address. `http://IPAddressHere` This is the default Web UI.
3. Now browse to the upgrade page. `http://IPAddressHere/up`
4. Click the third "Choose file" and select the "webui.html" file from the folder you unzipped earlier.
5. Click "Upload web."
6. If you see "OK" you are good to go!
7. You can power cycle your printer, but it's not necessary.
8. Once your printer is back online, browse to `http://IPAddressHere`. You should now have the upgraded Web UI.

## SD Card Functions

The file listing loads when the refresh icon is clicked. File names in the Web UI will be limited to 21 characters. The printer can support longer names, but it cuts off the extension and name after 24 characters.

Files that are uploaded will be renamed from "cache.gc" to the original file name. If you are re-uploading a previous file, the old file is deleted first, then the file is renamed. The .gc extension will be used to maximize file name length.

The print icon does two things: it selects the file `M32` for print, and tells the printer to print it `M24`, but it won't set the target tempatures. Pre-heat before requesting to print a file. Once the extruder and bed are at the target temperatures, the printer LCD will display the printing screen.

The delete icon will delete the file, `M30`, and refresh the file listing.

## Troubleshooting

Did something break? Here's how you can undo the Web UI upgrade.

1. Turn off the printer. Wait about 10 seconds and then turn it back on.
2. Once it's on and connected to Wi-Fi, browse to `http://IPAddressHere/up`.
3. Just click the "Upload web" button without choosing a file and this will restore the factory Web UI.

## Donation

If this project helps, you can buy me a cup of coffee. :grimacing: :coffee:

[![PayPal button](http://rawgit.com/twolfson/paypal-github-button/master/dist/button.svg)](https://www.paypal.me/thejoeycortez/5)