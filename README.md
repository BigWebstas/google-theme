# Google Theme

Home Assistant theme inspired by the Google Pixel (Material 3) light and dark interface.
<br />
<br />

[![hacs_badge](https://img.shields.io/badge/HACS-Default-orange.svg?style=for-the-badge)](https://github.com/custom-components/hacs)

<br />

## Screenshots

![Google Light Mode 1](https://raw.githubusercontent.com/BigWebstas/google-theme/main/images/Google_Light_Mode_1.jpg)<br />
<br />
![Google Dark Mode 1](https://raw.githubusercontent.com/BigWebstas/google-theme/main/images/Google_Dark_Mode_1.jpg)<br />
<br />

### Preparation
1. Make sure that under the **configuration.yaml** file you have the following:

```
frontend:
  themes: !include_dir_merge_named themes
```

2. Under the Home Assistant **Config** folder, create a new folder named **themes**
3. **Restart** Home assistant to apply the changes. 

### HACS installation
1. Go into the Community Store (HACS)
2. Search for **Google Theme**
3. Open the theme
4. Press Install
5. Restart Home Assistant

### Manual installation
1. In the Home assistant **themes** folder, create a file named `google_theme.yaml`
2. In this GitHub repo, go into the **themes** folder, open the `google_theme.yaml` file and copy the content
3. Paste the content in the `google_theme.yaml` file created under your Home Assistant themes folder

### Enable theme
1. Open your Home Assistant **Profile**
2. Under, **Themes**, select the new **Google Theme**

### Set theme as default for all devices
1. Open **Developer Tools**
2. Go to **Services**
3. Under **Service** enter `frontend.set_theme`
4. Under **Name**, enter `Google Theme`
5. Enable **Mode** and set it to `light`
6. Click on **Call Service**
7. Repeat steps 1 to 6 but change the **Mode** to `dark` 



