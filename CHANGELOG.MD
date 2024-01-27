(unreleased)
------------
- Sm8450-common: init: Deny access to HBM node. [Bruno Martins]

  The stock fingerprint sensor HAL writes to the HBM node on finger press,
  but that conflicts with UDFPS framework dimming. Do not let it mess
  things up.
- Sm8450-common: Fix system camera hack on martini. [LuK1337]

  This makes sure that last camera is marked as system camera.
- Sm8450-common: Unlock aux cameras. [LuK1337]

  This basically NOPs update_camera_metadata_entry() call that sets
  ANDROID_REQUEST_AVAILABLE_CAPABILITIES_SYSTEM_CAMERA to 1 for aux cams.
- Sm8450-common: Build HWC with UDFPS support. [pjgowtham]
- Sm8450-common: Rip feedback modules. [pppig236]

  useless debugging tool from oplus
- Sm8450-common: Switch to OSS composer. [pjgowtham]
- Sm8450-common: overlay: Set up UDFPS framework dimming. [dekefake]
- [DNM]Disable privapp-permissions whitelist enforcement. [Vineeta
  Srivastava]

  Otherwise device won't boot due to whitelist violations.
- Sm8450-common: Register wise light as android.sensor.light. [LuK1337]

  Sadly a lot of apps aren't aware of config_displayLightSensorType.
- Sm8450-common: Rip esim kmod. [pppig236]
- Sm8450-common: Do not build atrace HAL. [Pranav Vashi]


(unreleased)
------------
- Ovaltine: Kang auto brightness configs from Oneplus 8T. [Phạm Tiên
  Sinh]

  Originally, brightness in dim environment goes up and down when screen transitions from white to black and vice versa. This commit fixes that and also makes auto brightness more accurate.
- Ovaltine: Kang blobs from salami. [pppig236]


