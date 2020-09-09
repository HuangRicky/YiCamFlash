## Flashing Yi Camera to use in Home Assistant

# Background
Yi Camera is a nice surveillance tool. However, usually company would block rtsp or other feeds on their camera and only allow you to use proprietary tool, which is still very useful. In order to make it compatible with Home Assistant, you need to "hack" this hardware.

# Existing projects

Some expert have created the firmware file for Yi cameras.

https://github.com/TheCrypt0/yi-hack-v4

https://github.com/roleoroleo/yi-hack-Allwinner

# Installation on Yi Camera Home 1080p.

This is the official website link for Home 1080p cam.
[Yi Cam Home 1080p Link](https://store.yitechnology.com/products/yi-1080p-home-camera)

The issue is, if you buy the cam now, it's likely to get a cam with firmware version 8.2.0. So, you need to use https://github.com/roleoroleo/yi-hack-Allwinner , not "v4"

## Detailed steps
1. Need to download the Yi Home app on your cellphone.
2. Start pairing in your Yi Home App, click "Add" camera. Input your 2.4G Wifi network info (5G doesn't work!!!). Your App will show a QR code. Scan it with your Cam. Wait until your Cam shows blue light. Now you should be able to see your cam inside Yi Home app.

If you are satisfied with the original Yi Cam features, you can stop now.

3. Check your firmware's version in Yi Home App, in the camera, settings

3. Now follow https://github.com/roleoroleo/yi-hack-Allwinner instruction, suppose you have firmware version 8.2.0. I copy from Roleo's page:
4. Format an SD Card as FAT32. It's recommended to format the card in the camera using the camera's native format function. If the card is already formatted, remove all the files.
5. Download the latest release from the https://github.com/roleoroleo/yi-hack-Allwinner Releases page
6. Extract the contents of the archive to the root of your SD card. So that you will have 2 files on it.
7. Insert the SD Card and reboot the camera
8. Wait for the camera to update. It will reboot a couple of times as the camera is rooted and the new firmware is applied. It can take up to an hour to update. Once the light is solid blue for at least a minute it is complete. When it finishes, cam should show blue light.

9. Now, you can go to http://IP-CAM:8080  where your IP-CAM is your IP of camera. I find it in my Router's webpage


You can use the [editor on GitHub](https://github.com/HuangRicky/YiCamFlash/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/HuangRicky/YiCamFlash/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
