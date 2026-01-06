# AArch64 multi-platform
# Maintainer: Ray Sherwin <slick517d@gmail.com>
# Contributor: Kevin Mihelich <kevin@archlinuxarm.org>
# Contributor: Dragan Simic <dsimic@buserror.io>

pkgbase=linux
pkgver=6.16.0
pkgrel=1
_newversion=false
_stopbuild=false    # Will also stop if ${_newversion} is true
_srcname="linux-${pkgver/%.0/}"
_kernelname="${pkgbase#linux}"
_desc="AArch64 multi-platform with warpme patches"
arch=('aarch64')
url="http://www.kernel.org/"
license=('GPL2')
makedepends=('xmlto' 'docbook-xsl' 'kmod' 'inetutils' 'bc' 'git' 'dtc')
options=('!strip')
source=("https://git.kernel.org/torvalds/t/${_srcname}.tar.gz"
#source=("https://cdn.kernel.org/pub/linux/kernel/v6.x/linux-$pkgver.tar.xz"
0001-net-wireless-rtw88-fix-wrong-hw.ver.patch
0108-drivers-led-add-openvfd-g3118dda3.patch
0109-drivers-mmc-add-disk-activity-support.patch
0110-drivers-net-wireless-brcmfmac-add-ap6330-firmware.patch
0125-drm-lima-dvfs-switch-gov-to-performance.patch
0126-drm-panfrost-dvfs-switch-gov-to-performance.patch
0311-arm64-dts-meson-set-dma-pool-to-896MB.patch
0312-g12-set-cma-to-896MiB-for-4k.patch
0329-media-meson-vdec-esparser-check-parsing-.patch
0330-media-meson-vdec-implement-10bit-bitstre.patch
0331-media-meson-vdec-add-HEVC-decode-codec.patch
0332-media-meson-vdec-disable-MPEG1-MPEG2-hardware-de.patch
0341-arm64-meson-add-Amlogic-Meson-GX-PM-Suspend.patch
0342-arm64-dts-meson-add-support-for-GX-PM-and-Virtu.patch
0361-arm64-dts-meson-gxm-add-beelink-gt1.patch
0371-arm64-dts-meson-sm1-add-support-for-TX5-plus.patch
0377-drm-meson-swap-primary-overlay-zpos.patch
0500-clk-Implement-protected-clocks-for-all-OF-clock-prov.patch
0501-revert-clk-qcom-Support-protected-clocks-property.patch
0502-rtc-sun6i-Allow-RTC-wakeup-after-shutdown.patch
0503-firmware-arm_scpi-Support-unidirectional-mailbox-cha.patch
0504-mfd-add-AC200.patch
0505-net-phy-Add-support-for-AC200-EPHY.patch
0506-net-wireless-add-xr819-support-07072021.patch
0507-net-stmmac-sun8i-Use-devm_regulator_get-for-PHY-regu.patch
0508-net-stmmac-sun8i-Rename-PHY-regulator-variable-to-re.patch
0509-net-stmmac-sun8i-Add-support-for-enabling-a-regulato.patch
0510-iommu-sun50i-Allow-page-sizes-multiple-of-4096.patch
0511-drm-sun4i-de2-de3-Change-CSC-argument.patch
0512-drm-sun4i-de2-de3-Merge-CSC-functions-into-one.patch
0513-drm-sun4i-de2-de3-call-csc-setup-also-for-UI-layer.patch
0514-drm-sun4i-de2-Initialize-layer-fields-earlier.patch
0515-drm-sun4i-de3-Add-YUV-formatter-module.patch
0516-drm-sun4i-de3-add-format-enumeration-function-to-engine.patch
0517-drm-sun4i-de3-add-formatter-flag-to-mixer-config.patch
0518-drm-sun4i-de3-add-YUV-support-to-the-DE3-mixer.patch
0519-drm-sun4i-de3-pass-engine-reference-to-ccsc-setup-function.patch
0520-drm-sun4i-de3-add-YUV-support-to-the-color-space-correction-mod.patch
0521-drm-sun4i-de3-add-YUV-support-to-the-TCON.patch
0522-drm-sun4i-support-YUV-formats-in-VI-scaler.patch
0523-drm-sun4i-de2-de3-add-mixer-version-enum.patch
0524-drm-sun4i-de2-de3-refactor-mixer-initialisation.patch
0525-drm-sun4i-vi_scaler-refactor-vi_scaler-enablement.patch
0526-drm-sun4i-de2-de3-add-generic-blender-register-reference-functi.patch
0527-drm-sun4i-de2-de3-use-generic-register-reference-function-for-l.patch
0528-drm-sun4i-de3-Implement-AFBC-support.patch
0529-dt-bindings-allwinner-add-H616-DE33-bus-binding.patch
#0530-dt-bindings-allwinner-add-H616-DE33-clock-binding.patch
0531-dt-bindings-allwinner-add-H616-DE33-mixer-binding.patch
0532-drm-sun4i-de33-mixer-add-Display-Engine-3.3-DE33-support.patch
0533-drm-sun4i-de33-vi_scaler-add-Display-Engine-3.3-DE33-support.patch
0534-drm-sun4i-de33-fmt-add-Display-Engine-3.3-DE33-support.patch
0535-drm-sun4i-de33-csc-add-Display-Engine-3.3-DE33-support.patch
#0537-clk-sunxi-ng-ccu-add-Display-Engine-3.3-DE33-support.patch
0538-add-TCON-global-control-reg-for-pad-selection.patch
0540-drm-bridge-dw-hdmi-add-mtmdsclock-parameter-to-phy-c.patch
0541-drm-bridge-dw-hdmi-support-configuring-phy-for-deep-.patch
0542-drm-sun4i-dw-hdmi-Switch-to-bridge-functions.patch
0547-drm-dw-hdmi-cec-sleep-100ms-on-error.patch
0548-drm-bridge-dw-hdmi-fix-4k60-modes-on-some-tv.patch
0549-drm-bridge-synopsys-Fix-CEC-not-working-after-power.patch
0550-HACK-clk-sunxi-ng-unify-parent-for-HDMI-clocks.patch
0552-asoc-sun4i-i2s-WiP-multi-channel.patch
0553-media-cedrus-Don-t-CPU-map-source-buffers.patch
0554-media-Add-NV12-and-P010-AFBC-compressed-formats.patch
0555-media-cedrus-add-format-filtering-based-on-depth-and.patch
0557-media-cedrus-Increase-H6-clock-rate.patch
0560-mmc-sunxi-fix-unusuable-eMMC-on-some-H6-boards-by-di.patch
0561-bluetooth-btrtl-add-hci-ver-rtl8822cs.patch
0562-h6-add-sun50i-di-deinterlace-WiP.patch
#0563-hantro-Add-quirk-for-NV12-NV12_4L4-capture-format.patch
0570-arm64-dts-allwinner-h6-Protect-SCP-clock.patch
0571-arm64-dts-allwinner-h6-Add-SCPI-protocol.patch
0572-arm64-dts-allwinner-h6-dtsi-add-sound-node.patch
0573-arm64-dts-allwinner-h6-Fix-Cedrus-IOMMU-again.patch
0574-arm64-dts-allwinner-h6.dtsi-add-ac200-nodes.patch
0575-arm64-dts-allwinner-gs1-fixes.patch
0576-arm64-dts-allwinner-tanix-tx6-additions.patch
0577-arm64-dts-allwinner-add-Eeachlink-H6-Mini.patch
0580-arm64-dts-allwinner-opi3-fixes.patch
0582-arm64-dts-allwinner-h6-add-deinterlace-node.patch
0583-arm64-dts-allwinner-add-orangepi-3-lts.patch
0600-drivers-h616-wip-add-usb-emac2-support.patch
0601-drivers-thermal-allwinner-add-h616-ths-support.patch
0602-media-cedrus-add-H616-variant.patch
0603-soc-sunxi-sram-Add-SRAM-C1-H616-handling.patch
0604-dma-sun6i-dma-add-h616-support.patch
0610-drm-sun4i-add-sun50i-h616-hdmi-phy-support.patch
0615-drivers-iommu-sun50i-iommu-fix-iommu-on-h616.patch
0620-sound-soc-sunxi-add-codec-driver-for-h616.patch
0621-sound-soc-add-sunxi_v2-for-h616-ahub.patch
0623-sound-soc-sunxi-hack-to-fix-oops-on-cards-caps-query.patch
#0630-net-wireless-add-uwe5622-support-v20231020.patch
0631-clk-sunxi-ng-ccu-sun6i-rtc-fix-32k-clk.patch
0632-clk-sunxi-ng-ccu-hack-fix-too-slow-hdmi-audio.patch
0633-regulator-add-mmc-high-speed-SD-UHS-modes-support.patch
0635-drvers-of-add-dt-overlay-configfs-interface.patch
0640-arm64-dts-allwinner-h616.dtsi-add-audio-hdmi-vdec.patch
0641-arm64-dts-allwinner-h616.dtsi-add-cpu-gpu-dvfs-opp.patch
0642-arm64-dts-allwinner-h616.dtsi-add-emac1.patch
0643-arm64-dts-allwinner-h616.dtsi-fix-x96q-failing-mmc3.patch
0644-arm64-dts-allwinner-h616.dtsi-enable-highspeedx-on-mmc0.patch
0644-arm64-dts-allwinner-h616-OrangePI-Zero23-enable-ths-hdmi-audio.patch
0645-arm64-dts-allwinner-h616-add-Tanix-TX6s-TVbox.patch
0646-arm64-dts-allwinner-h616-add-Tanix-TX6s-axp313-TVbox.patch
0647-arm64-dts-allwinner-h313-add-x96q-TVbox.patch
0648-arm64-dts-allwinner-h313-add-x96q-lpddr3-TVbox.patch
0649-arm64-dts-allwinner-h618-add-vontar-h618-TVbox.patch
#0650-arm64-dts-allwinner-h618-add-opi-2w.patch
0650-arm64-dts-allwinner-h618-improve-opi-2w.patch
0651-arm64-dts-allwinner-h313-improve-tanix-tx1.patch
0652-arm64-dts-allwinner-h313-add-x96q-v5.1-TVbox.patch
0653-arm64-dts-allwinner-h616-add-pendoo-x12pro-tvbox.patch
0654-arm64-dts-allwinner-h618-improve-transpeed-8k618-tvbox.patch
0655-arm64-dts-allwinner-h313-h616-h618-add-cpu-overclock-via-overlays.patch
0656-arm64-dts-allwinner-h313-h616-h618-add-gpu-overclock-via-overlays.patch
0722-v4l2-wip-iep-driver.patch
0725-drm-rockchip-vop-add-immutable-zpos-property-fix-z-order.patch
0727-drm-rockchip-vop2-rk356x-reorder-wins-fix-osd-in-drm-planes.patch
0738-arm64-dtsi-rockchip-rk3399-rise-alert-crit-cpu-temps.patch
0739-arm64-dtsi-rockchip-rk3328-rk3399-add-soft-reset.patch
0740-arm64-dts-rockchip-var-fixes-from-libreelec.patch
0743-arm64-dts-rockchip-beelink-a1-enable-openvfd.patch
0746-arm64-dts-rockchip-beelink-a1-bump-cpu-gpu-freqs.patch
0747-arm64-dts-rockchip-beelink-a1-limit-sdmmc-clk-to-35MHz.patch
0748-arm64-dts-rockchip-beelink-a1-limit-emmc-speed-to-fix-emmc-booting.patch
0749-phy-rockchip-phy-add-rockchip-inno-usb3.patch
0750-arm64-dts-rockchip-rk3328-enable-inno-usb3-on-various-boards.patch
0753-arm64-dts-rockchip-rk3399-radxa-rockpi-bc-remove-wifi-compatible.patch
0754-arm64-dts-rockchip-rk33xx-set-userled-to-mmc.patch
0755-arm64-dts-rockchip-rk3399-add-orangepi-4-and-4-lts.patch
0756-arm64-dts-rockchip-rk33xx-add-eth-wifi-aliases.patch
0757-arm64-dts-rockchip-rk3399-orangepi-4-lts-add-fan-support.patch
0758-arm64-dts-rockchip-rk3328-rk3566-add-cpu-gpu-overclock-overlays.patch
0800-Enable-rk356x-PCIe-controller.patch
0801-net-wireless-backport-aic8800-sdio-v2025_0410_gb99ca8b6-mm2.patch
0803-net-wireless-backport-aic8800-usb-v2025_0410_gb99ca8b6-mm2.patch
0831-arm64-dts-rockchip-enable-usb2-usb3-sata-audio-in-rk35xx.dtsi.patch
0832-arm64-dtsi-rockchip-rk356x-disable-vepu-rga-enable-dfi.patch
0833-arm64-dts-rockchip-enable-Quartz64-A-usb2-usb3-pcie-audio.patch
0836-arm64-dts-rockchip-add-dts-for-x96-x6.patch
0840-arm64-dts-rockchip-improve-dts-for-rock3b.patch
0841-arm64-dts-rockchip-increas-alarm-cpu-temp-to-85.patch
0842-arm64-dts-rockchip-Quartz64-B-fix-Eth-enable-hdmi-audio.patch
0843-arm64-dts-rockchip-rock3a-fix-mdio-reset-disable-uart-bt.patch
0845-arm64-dts-rockchip-improve-dts-for-rock3c.patch
0846-arm64-dts-rockchip-rk35xx-set-userled-to-mmc.patch
0847-arm64-dts-rockchip-add-dts-for-urve-pi.patch
0848-arm64-dts-rockchip-add-dts-for-opi-3b.patch
0849-arm64-dts-rockchip-improve-dts-for-zero3.patch
0850-arm64-dts-rockchip-rk356x-add-eth-wifi-aliases.patch
#0900-rpi-vc04_services-add_h~l2-m2m_decode-15062024.patch
#0902-media-add-rpivid-driver.patch
#0932-drivers-pci-add-rp1-support.patch
#0933-drivers-clk-add-rp1-support.patch
#0934-drivers-pinctrl-add-rp1-support.patch
#0935-drivers-dma-add-rp1-support.patch
#0936-drivers-irqchip-add-rp1-support.patch
#0937-drivers-phy-add-rp1-support.patch
#0938-drivers-mfd-add-rp1-support.patch
#0939-drivers-pmdomain-add-rp1-support.patch
#0940-drivers-mmc-add-rp1-support.patch
#0941-drivers-i2c-add-rp1-support.patch
#0942-drivers-usb-add-rp1-support.patch
#0943-drivers-net-add-rp1-support.patch
#0944-drivers-spi-add-rp1-support.patch
#0945-drivers-pwm-add-rp1-support.patch
#0946-drivers-hwmon-add-rp1-support.patch
#0947-drivers-thermal-add-rp1-support.patch
#0948-gpu-drm-vc4-add-rpi5-support.patch
#0948-gpu-drm-vc4-sync-to-rpi-downstream.patch
#0949-drivers-iommu-add-bcm2712-iommu.patch
#0970-arm64-dts-brcm-rpi4-set-led-to-disk-activity-mmc0-alias.patch
#0971-arm64-dts-brcm-rpi5-add-rp1-usb-eth-pwm.patch
#0972-arm64-dts-brcm-rpi5-fix-hdmi-audio.patch
#0973-arm64-dts-brcm-rpi5-add-v3d.patch
#0974-arm64-dts-brcm-rpi4-add-rpivid.patch
#0975-arm64-dts-brcm-rpi5-add-rpivid.patch
#0976-arm64-dts-brcm-rpi5-add-iommu.patch
#0977-arm64-dts-brcm-rpi5-incr-cma-to-384M.patch
#0978-arm64-dts-brcm-rpi5-add-fan-support.patch
#0979-arm64-dts-brcm-rpi4-incr-cma-to-384M.patch
#0980-arm64-dts-brcm-rpi5-add-wifi-bt-support.patch
#0981-arm64-dts-brcm-rpi5-add-leds-aupport.patch
1003-math.h-add-DIV_ROUND_UP_NO_OVERFLOW.patch
1004-clk-divider-Fix-divisor-masking-on-64-bit-platforms.patch
1005-clk-composite-replace-open-coded-abs_diff.patch
1006-watchdog-dw_wdt-fix-default-timeout.patch
1007-PM-devfreq-rockchip-dfi-double-count-on-RK3588.patch
1008-mfd-rk8xx-Fix-shutdown-handler.patch
1009-drm-rockchip-vop2-rk3588-reorder-wins-fix-kodi-playback-in-drm-planes.patch
1016-dt-bindings-display-vop2-Add-VP-clock-resets.patch
1017-drm-rockchip-vop2-Add-clock-resets-support.patch
1018-drm-rockchip-vop2-Add-core-reset-support.patch
1020-WIP-drm-rockchip-dw_hdmi_qp-Make-use-of-phy_configur.patch
1030-WIP-drm-bridge-Add-detect_ctx-hook.patch
1031-WIP-drm-bridge-connector-Switch-from-detect-to-detec.patch
1032-WIP-drm-bridge-dw-hdmi-qp-Add-high-TMDS-clock-ratio-.patch
1033-dt-bindings-display-rockchip-Add-schema-for-RK3588-D.patch
1034-drm-bridge-synopsys-Add-DW-DPTX-Controller-support-l.patch
1035-drm-rockchip-Add-RK3588-DPTX-output-support.patch
1036-dt-bindings-display-simple-bridge-Add-ra620-compatib.patch
1037-drm-birdge-simple-bridge-Add-support-for-radxa-ra620.patch
1038-drm-bridge-synopsys-add-cec-support.patch
1039-net-ethernet-add-yt6801-gige-pcie-controller.patch
1040-net-ethernet-yt6801-gige-pcie-silence-debug-msgs.patch
1041-net-stmmac-dwmac-rk-fix-disabling-set_clock_selection.patch
1054-bitmap-introduce-hardware-specific-bitfield-operatio.patch
1055-media-rkvdec-Restore-iommu-addresses-on-errors.patch
1056-media-dt-bindings-rockchip-Document-RK3588-Video-Dec.patch
1057-media-dt-bindings-rockchip-Add-RK3576-Video-Decoder-.patch
1060-media-uapi-HEVC-Add-v4l2_ctrl_hevc_ext_sps_rps-contr.patch
1061-media-v4l2-ctrls-Add-hevc_ext_sps_rps-control.patch
1062-media-rkvdec-Remove-TODO-file.patch
1063-media-rkvdec-Unstage-the-driver.patch
1067-media-rkvdec-Switch-to-using-structs-instead-of-writ.patch
1068-media-rkvdec-Move-cabac-table-to-its-own-source-file.patch
1069-media-rkvdec-Use-structs-to-represent-the-HW-RPS.patch
1070-media-rkvdec-Move-h264-functions-to-common-file.patch
1071-media-rkvdec-Add-per-variant-configuration.patch
1072-media-rkvdec-Add-RCB-and-SRAM-support.patch
1073-media-rkvdec-Support-per-variant-interrupt-handler.patch
1074-media-rkvdec-Enable-all-clocks-without-naming-them.patch
1075-media-rkvdec-Add-H264-support-for-the-VDPU381-varian.patch
1076-media-rkvdec-Add-H264-support-for-the-VDPU383-varian.patch
1077-media-rkvdec-Add-HEVC-support-for-the-VDPU381-varian.patch
1078-media-rkvdec-Add-HEVC-support-for-the-VDPU383-varian.patch
1079-media-rkvdec-fix-10bit-playback.patch
1080-arm64-dtsi-rk3588s-add-vop2-clock-resets.patch
1081-arm64-dtsi-rockchip-add-dw-dp-nodes.patch
1082-arm64-dts-rockchip-Add-the-vdpu381-Video-Decoders-on.patch
1083-arm64-dts-rockchip-Add-the-vdpu383-Video-Decoder-on-.patch
1084-arm64-dtsi-rockchip-rk356x-add-rkvdec2-video-decoder-nodes.patch
1087-arm64-dts-rockchip-rk3588s-rock5a-dts-improvements.patch
1088-arm64-dts-rockchip-rk3588-rock5b-dts-improvements.patch
1089-arm64-dts-rockchip-rk3588s-rock5c-dts-improvements.patch
1090-arm64-dts-rockchip-rk3588-rock5itx-dts-improvements.patch
1091-arm64-dts-rockchip-rk3588s-opi5-dts-improvements.patch
1092-arm64-dts-rockchip-rk3588-opi5plus-dts-improvements.patch
1093-arm64-dts-rockchip-rk3588s-add-opi5pro-dts.patch
1094-arm64-dts-rockchip-rk3588s-add-nanopi-m6-dts.patch
1095-arm64-dts-rockchip-rk3588s-nanopc-r6s-dts-improvements.patch
1096-arm64-dts-rockchip-rk3588-nanopc-t6-dtsi-improvements.patch
1097-arm64-dts-rockchip-rk3588-add-rock5t-dt.patch
1099-arm64-dtsi-rockchip-disable-vpu121.patch
1100-clk-sunxi-ng-a523-Mark-MBUS-clock-as-critical.patch
1101-axp20x-HACK-mfd-and-multiple-axp-on-the-bus.patch
1103-allwinner-a523-Add-power-controllers.patch
1104-regulator-axp20x-force-polyphase-setup-for-axp323.patch
1140-net-drivers-stmmac-add-initial-support-for-a523-gmac1.patch
1141-thermal-drivers-sun8i-add-initial-support-for-ths-v2.patch
1142-add-initial-cpufreq-support.patch
1151-arm64-dtsi-allwinner-add-gmac1-fixup-gmac0-in-a523.patch
1153-arm64-dtsi-allwinner-add-ths-support-v2.patch
1154-arm64-dtsi-allwinner-add-cpufreq-support.patch
1155-arm64-dtsi-allwinner-add-gpu-support.patch
1170-arm64-dts-allwinner-h728-x96q-pro-plus-improvements.patch
1172-arm64-dts-allwinner-t527-add-orangepi-4a-dts.patch
1173-arm64-dts-allwinner-a527-Radxa-A5E-improvements.patch
1205-thermal-rockchip-rename-rk_tsadcv3_tshut_mode.patch
1206-thermal-rockchip-Support-RK3576-SoC-in-the-thermal-driver.patch
1207-thermal-rockchip-support-reading-trim-values-from-OTP.patch
1209-PM-devfreq-rockchip-dfi-add-support-for-LPDDR5.patch
1211-drm-rockchip-dw_hdmi_qp-provide-ref-clock-rate-in-dw_hdmi_qp_plat_data.patch
1212-drm-bridge-dw-hdmi-qp-fixup-timer-base-setup.patch
1213-net-phy-realtek-reset-after-clock-enable.patch
1214-mmc-core-add-force-io-to-1.8v-quirk.patch
1260-arm64-dtsi-rockchip-fix-hdmi-output-on-rk3576.patch
1265-arm64-dtsi-rk3576-add-sdio-node.patch
1266-arm64-dtsi-rockchip-Add-thermal-nodes-to-RK3576.patch
1267-arm64-dtsi-rockchip-Add-thermal-trim-OTP-and-tsadc-nodes.patch
1268-arm64-dtsi-rockchip-enable-RK3576-watchdog.patch
1280-arm64-dts-add-rk3576-nanopi-m5-dt.patch
1281-arm64-dts-rock4d-improvements.patch
1282-arm64-dts-add-rk3576-nanopi-r76s-dt.patch
	config
        linux.preset)
#        60-linux.hook
#        90-linux.hook)

md5sums=('08ab460ca3a1d9210f5b7c2549b6bad3'
         '67fd36bdd6b72b2cca18fe617f86a47e'
         'ad0019ba412a1b4f54fc413e2c5c3e76'
         'e0e2176d175d13f56da374df109e70e1'
         'e2706a83da3208d8c2735a482aab4ce9'
         'b3784de0372d33af27d09b521e777cab'
         'b142e3ad8d62036e6726659542c831db'
         'd5de63e2a428f90ae624bfbe62eb473c'
         '4e8fc6412d17706efb885bf32d9d5d7b'
         '111511a711065179b3bbc09d4dc2530b'
         '4c2b514f5d212529d7c44540a553fbd4'
         'f775b1a8b7f714ca99ec14a04da89811'
         '4f7e219ddf5cde8bf4a00ceaaaad4bc1'
         'e6a64152bae9e70d520fa8f4ab40cea5'
         '5d038553c354cf2d6eafd51c42678207'
         '1580db9f84e0a45f0c56e8493d74a180'
         'fcd353d7ec30ada2446b2e75508378ea'
         'afe45a893ba82626813bc54cc0675cc6'
         '98cca6a3cb864b1f06022d145761445b'
         '475e6eccc1d647ccfb030c24e1f89a89'
         '4668886e40c0c9bc2ea4f62868803e4a'
         'a7e8181374ada3419a3922c4e10d46da'
         'e9d5b81c6db0a2e3724f02ca9c52d25a'
         '59d800179f06078caf4e202291985f4b'
         '5f73f77065196e91f2e4455388bb454f'
         '082667b0867720fcc338f8cf93cc7314'
         '7ed076b3fc61d2a405934d301ecf1643'
         '440cb89d09ccb6ac72bff2ae811f1950'
         'e4547a0f96133ca4217f480886e7e1fd'
         'b0d035957a88de4e6d5eaba2c8ada082'
         'ca7a61f60e825699f3031a45dad56132'
         '7400b7db8778f454ae9bc80ca4c09c8b'
         'a051ec00bfde18435034545dda1593e8'
         '4d1a5fd7203b519c3aa775d9588a5de5'
         'eca8ab7fd2a4021a903eea1463334fc7'
         'b5a047aedb19ada2783324a4ca5c45e2'
         'dbddf467256680e6ce09eac909a5f634'
         'ae8c45134acd34a5b786417d0faa0077'
         '950a1d64631a422d91b7718d162ef217'
         '7f2f60b406faab52303781b5e7fbd0b9'
         'ec8b6d0dfc30970eab5906aaaefacb63'
         '3b963ac322083744503e82a3a3c7ca98'
         'ef4b038799f9a0cdf02a5dd392233979'
         '56f742021db4bc4160346ac8c13557f6'
         '8b2a36364094931fc607ccda4dbbe1c9'
         'a1d69960c0d7f1bef0fdb049562225d7'
         '1540f61bbc0528f2da6e4e3ff99aabdb'
         'ad50a1423a448bc225e6e04996e0d78e'
         '06894edca0de3d1965402e6e72c70f22'
         '49d7ccf91b924ad431a8a2d62ecf6312'
         '1cabd78bf15d3d119fb124eaa5e808fb'
         '9c8e33ad442761113f3ffe7f7a58e373'
         'db0ff6d26ea19b4a8360841c3bf76b0b'
         '99e4a65fbe05aca0da04ae55c5a0ca9f'
         '1f1d8ae4ede5f0679310b65076749a2e'
         'c3e9d498c6b413e157433d6a509a81b4'
         '00f270a9b79820fec143e8387f8bc444'
         '7377e24f367aefded32626d68036637f'
         'e4a4657990a54cdc00f8ecb322aa6049'
         '630efe044f9ec1d3a7c4cc6a15c4219a'
         '8488af1e862c67cf7e41753b96aeea6b'
         '1699b20e867741a86c35d743b4a17df4'
         '95b517e62538ac03f522e8a5b3660fb8'
         '874b8b9b17ffd156d4f0dfa4b1a5e81e'
         '39790f191e61387817480a50899600a9'
         '4f0853228839336c69adcb2d9dadf2b3'
         '0e6ebee7a6c045dd7cf45cbafbf924bb'
         '1dcafc57cdbc3421e12ab54a54c8284c'
         'f912776f05276c66311105f57fb5d475'
         'fac6a4de3708bb8a2423a12a592120bb'
         '554fd010bfcfd195deeaaa5a180499b9'
         'cb47353acc35d5ef90d2c4a1f51ef6e1'
         'ff3e22baa0060cbc6b8d7956b166680e'
         'aa19151df8770f0fa126a93fade5d115'
         '2311d1b0063b0ecbb222fa1449872891'
         '15cee9e21ff6bdd2359496cd0aafa280'
         '2a8daf86328b8ae4e7fb875652dc19d2'
         'e3a0b0484fd17975620289818fc9c885'
         'e2bf8a4a8706706ef53879c6e0238db4'
         '97b02760dd91244d39094574d8256750'
         '92ffc7f9614867c1e229aa80c41395df'
         '42db2fae3d4fc7435de7f756d12d456c'
         '63e44cc95a8b2ede6a5f8ee830e795bc'
         '226ff38d2a1ead67c4457210b2f8f42f'
         '590861813b731c3783645007146b0d09'
         'a87199b148b4c189aedd93ada88c4152'
         'cf9d1002d2e87982a37730fbdda23ab0'
         'a36846f6e57848bd58065aaf55c32c23'
         '2b5ffe71dd9b653df00d04819c71ac25'
         'a60e60823753eb54c85af4214c9cb104'
         'f68f47d2728f964b399f5ee302f4aaeb'
         'cdad029e1ba91f4182efd3f4d7b1aa89'
         '5ee50f81c91e37c7ebab799b6be333dc'
         '4257bf04a0e285d6caeb4a3e1519226f'
         'c5eb21b3b6f59b2a37d2cc4c8f68701f'
         '85811e3a1b99e3d562c0453ec53b0a9b'
         'abe67e12862f6aab45af666d27a689ae'
         '2322b63bd374e80189211273b5e21785'
         'e873e4f3dd135e6920738013f1685e97'
         'f5f429d04a1d8103610217f2f4d5f2a2'
         '4c4ba44d4a008a6ca658c785f711db65'
         '1dcdf886ea8bdd6cf8cb4f61a4bea0d8'
         '4e3a3740e9fe6a792f941ff83a33ad73'
         '75db156ff48a2dd84dfd3a7b7ccba1c9'
         'd8cb7020ff0a0bf7b01412b31e791046'
         '9b708485dd208e4fd38278226d1665e4'
         'b7870188262be5039ac14e187b691276'
         '3bf673c93292aa953ba925e882cfb2cb'
         '9727a438eca6477b7ecdf28d43a35553'
         '8a387289e6084ea76da96b30fd02ec0e'
         '06beea3fd0bc8985da22bc0f9d224c96'
         'a06129a8cf6a487e65af60c85aacb5ab'
         '031646e4ddde55979488a7c9f44fe76d'
         'e7ae0a54c830f35a9eb41f8db035fc68'
         '9e8cb8822f2db5b3a62edb39ff3f94e9'
         '01b30e73433381d060319c283017a3c7'
         '6408cd90546123bd07f4f80f2b7010e3'
         '87fa225131a0ce93e88503b04543bd39'
         'c891fba63f548409549b1a96d8604680'
         '9a2c9408381d546b16e983246484fd40'
         'da75c3163ffef13cbe070ed1d75da4e3'
         '84eeeb28c18b434dbf72ba3ed5f759b2'
         'f72cde7a7e37974c60abc6db7f8e5340'
         'a0cebbf223a6f4bb5cc087ad46faa73e'
         '12f1da0a3013cbbd6a4724490dbc99d1'
         '0915610e97e58b4cdb9a5c4cdbd54a2f'
         'fbd3050b4a357d249e758c7220a14320'
         '148de4dd254cd9b1b514cf96e7cf07f3'
         '5596eed0396b37cd7a89ded4e3d2105d'
         'be841c057f24c034311a4a634ddaaa61'
         '36f183da40a11eaf6245b12aa0092684'
         '202a70aa12b06bf82540577844d59d7c'
         '742095da417466f354223106ac390d1e'
         'ca782317804d7eca9aad74f2dcdc12a0'
         'e87f12a7315571bdb20092be976dea69'
         'aa82f20d5d6ec8affc6915058c2d4ab2'
         'd559a352374a2becd9fb6d30c6c7b6cf'
         '6b514cb03ef096d5d2f42a8b4332d918'
         '94a9317c40a68c10504f492a0abf72da'
         '7ff3b7e09aaefa3060fb18a6bc04d367'
         '0f38739e23894da7251ee14e35bed22b'
         'b4540ed9cd9ae1a1d45b7f3147aabf07'
         '9a325a4e8febfdd8b13b3713be3a30a4'
         '48c85cf2e1b0df6bd0f8c73525e1d999'
         '8979801afff6e1407ecb61d7a7de8652'
         '05d1980ebf3f2c5bec748615d8de5e31'
         '59fa47be5f410dc12516b03a7212b0e4'
         'f06731cfb7b2812d6d4d125d13ceca70'
         'fc4908203b9799983494bcfb7db0503e'
         '6425b1cb85e02afb1d901fba7ce67316'
         'c7979100005cd403bf2b93357ce42c4d'
         '38f19492d2c4490357624ed6392d78ea'
         '8fd57b490ce42f7e92bbd5c170133185'
         '9513f9b895fdb79167581c935cea06c1'
         '13d55b469c784a5aec977a3578377852'
         '9fe4b5a243141e12b7e34a8e13b56148'
         '4c3db6c8543c297d751b57755bbcc569'
         '8d6c800c8c24bb8c5db5f2cdd35d9ce0'
         '303760696acf1f674d663b7d19e5ae15'
         '4a43851b350aa5838c3a9d2062759625'
         '2a662945082e1c33c70cc133497b70f8'
         '524859aa28f1e070fe5d1f14baaa4e8f'
         '82f519d53438e9cde3d809893353988c'
         'd93d74461450446a26356b3f0fcf3462'
         'd61e30794d7476635ab1c737f2945f60'
         '5e8b415174ba6186f8412142d2234b6f'
         '85a40e7b98addf0f7499de367fc6518f'
         '7d653321ae7f79d08bbd58e4ac1def0b'
         '3502eb8a17aacac3df37c941461162f8'
         '888eb4f62dc8aea365ad4827ee16f319'
         '657d9cb461f204b5ec515a30e1300625'
         'b78b448b6ee1c42aad79134401f6f588'
         '2fe74619081bf5e8657cc8696ad4577b'
         '6e54fafa896f6c0f39202ba4bf3b1e77'
         '26ccc0099fe736052457facad757cd10'
         '7278bb1e4d68e04cb22a746a4b1e3ae6'
         '3101a13eefe04abeb8edaea019ae24ec'
         '519232fdac1957b72c370964e4b18950'
         '1742a541f1f4e8b1dc7f8d637804a230'
         'be8ee894267f449f589bc31b4b708612'
         'e6846fa0997f891c73e3f2a460343513'
         'aec1c788b2ea5c4a3cbef748dc54bec6'
         '85fd409d33f327828983332701d0b366'
         '1f9ffb86c636e13046e22d699632d6b0'
         'ba94255375d83cd99856fba71e9625fb'
         '40f71386adebc24c27264497a09d2d31'
         'b0a561b05aa918fc441a5c11488aec06'
         '22348cac10e10717c72df6ee2e704411'
         '7b19cb6cd3f47ddc16eaabfe37edda98'
         '8b3ffc800ffeb0cd8af5bfcb13d1a8b6'
         'ccc1d99dadd671d5ba5ef19b4e493367'
         '5ad2f4fae8d1e947dd98915eefe0bbe1'
         '13c64072621cb9a343f893b733ca1ed6'
         'ee547b715442e4cd317965acf7cde35a'
         '4b95bfff08c932f60e91a50c82be8934'
         '4b92fdb7fe252913207fa41e5dd89561'
         'e87c97f1ea8d7e099664dce90ba27930'
         '7a436ae28c30215dacf088bd53452304'
         '93531742c48d4712912a9504dd605c85'
         'a350915308a044704df9a2e207288e36'
         'e1c03826ab3db7bb89a873b377b46ef1'
         'c1e3e3e980c1c491aa7a0344d4c3734c'
         '4be073f2f73e5a6e5b3dedfc5dce1d4a'
         '097d9c47a265d9cb96e06751101c50e1'
         'cafc8d4a33fedfc997f5034c85685f77'
         '2d8abeb75fb7e2887df8adf319d81976'
         '0ebc406ec892d060cf073c968ee695a6'
         'e090aaa01e51fb7899c23093c970c0ed'
         '1bae78382a2f4d7ea7ced8230af9b204'
         'b6ed48d9144aae58964ec058214e4429'
         '0611260b581eab21230592f129811b44'
         '05a29ce2f04250c9db78c1e0cb17e56c'
         'c2433dccbf49896f9ea109108e69a41c'
         '4289244783840e6ec809300dbc981918'
         '2359c12aacf040124ff5a68b0bcf348a'
         '9010b2154fe2c9b5c5b56f198987288c'
         '6bb9a0762fcc7b600d726db1e7466fc4'
         'dfc0a51a332c23d6ef41db60268ce5ec'
         'c3983a09481b1717f2417b73263783d9'
         'e91fa37dfe50e4d5c3156e97f2cca235'
         '8cc812d646a10c5ec6c5282461e643a5'
         '640981f67803e3fbd08ab498e3f1b96e'
         'e735c34cbaf507a68fcf3d25334413da'
         '2542e93893b9655af88a6f314f55211e'
         '8869630655b15dee3abb2a357007e028'
         '81de5c287434b45e46867f89ef20ac38'
         '5dcec57d1d25d8dad20a66349ac0abcd'
         '01d8e852243ca83bf4a758b275bc2bd1'
         '98ac6e449b13696c5a5217689b6c1c7c'
         '6d337c843f9277bf4e405ecd9f48fdb6'
         '95d6ed35d7750be162d0e68e8a8e6014'
         'a1e6842bb282803b52d5aff020e299e8'
         'dc7516ebd22c5f039a0e73b5bb89b901'
         'be833a2017b44f26eb0ae5707d65f736'
         '951f28a0ad253c8e05046bc1b73fb083'
         '1f61fd7ece5404b5adf3a456eca27cbf'
         '6df21ef00c4502631b600dc9d9567aa7'
         'f141008cbab59082c1b0d94883058296'
         'fcb78ef09e5865d021d1ddfece83c93d'
         '86d4a35722b5410e3b29fc92dae15d4b')

prepare() {
  apply_patches() {
      local PATCH
      for PATCH in "${source[@]}"; do
          PATCH="${PATCH%%::*}"
          PATCH="${PATCH##*/}"
          [[ ${PATCH} = $1*.patch ]] || continue
          msg2 "Applying patch: ${PATCH}..."
          patch -N -p1 < "../${PATCH}"
      done
  }

  cd ${_srcname}

  # Assorted Manjaro ARM patches
  apply_patches 0
  apply_patches 1

  # Assorted Pinebook, PinePhone and PineTab patches
#  apply_patches 2

  # Assorted RK35XX patches not yet upstreamed
#  apply_patches 3

  # Pinebook Pro patches by Megi
#  apply_patches 4

  # Apply our kernel configuration
  cat "${srcdir}/config" > .config

  # Add pkgrel to extraversion
  sed -ri "s|^(EXTRAVERSION =)(.*)|\1 \2-${pkgrel}|" Makefile

  # Don't run depmod on "make install", we'll do that ourselves in packaging
  sed -i '2iexit 0' scripts/depmod.sh
}

build() {
  cd ${_srcname}

  # Get the kernel version
  if [[ "${_newversion}" = false ]]; then
    make prepare
  fi

  # Configure the kernel; adjust the line below to your choice
  # or simply manually edit the ".config" file
  if [[ "${_newversion}" = true ]]; then
    make menuconfig   # CLI menu for configuration
  fi
  #make nconfig       # New CLI menu for configuration
  #make xconfig       # X-based configuration
  #make oldconfig     # Using old config from previous kernel version

  # Stash the configuration (use with new major kernel version)
  if [[ "${_newversion}" = true ]]; then
    cp ./.config /var/tmp/${pkgbase}.config
    cp ./.config "${srcdir}/config"
  fi

  # Stop here, which is useful to configure the kernel
  if [[ "${_newversion}" = true || "${_stopbuild}" = true ]]; then
    msg "Stopping build"
    return 1
  fi

  # Enable to create an all-inclusive build
  #yes "" | make config

  # Build the kernel and the modules
  unset LDFLAGS
  make ${MAKEFLAGS} Image modules

  # Generate device tree blobs with symbols to support
  # applying device tree overlays in U-Boot
  make ${MAKEFLAGS} DTC_FLAGS="-@" dtbs
}

_package() {
  pkgdesc="The Linux Kernel and modules - ${_desc}"
  depends=('coreutils' 'kmod' 'initramfs')
  optdepends=('crda: to set the correct wireless channels of your country'
              'linux-firmware: additional firmware')
  provides=('kernel26' "linux=${pkgver}")
  conflicts=('kernel26' 'linux')
  backup=("etc/mkinitcpio.d/${pkgbase}.preset")
  install=${pkgname}.install

  cd ${_srcname}

  KARCH=arm64

  # get kernel version
  _kernver="$(make kernelrelease)"
  _basekernel=${_kernver%%-*}
  _basekernel=${_basekernel%.*}

  mkdir -p "${pkgdir}"/{boot,usr/lib/modules}
  make INSTALL_MOD_PATH="${pkgdir}/usr" modules_install
  make INSTALL_DTBS_PATH="${pkgdir}/boot/dtbs" dtbs_install
  cp arch/$KARCH/boot/Image "${pkgdir}/boot"

  # make room for external modules
  local _extramodules="extramodules-${_basekernel}${_kernelname}"
  ln -s "../${_extramodules}" "${pkgdir}/usr/lib/modules/${_kernver}/extramodules"

  # add real version for building modules and running depmod from hook
  echo "${_kernver}" |
    install -Dm644 /dev/stdin "${pkgdir}/usr/lib/modules/${_extramodules}/version"

  # remove build and source links
  rm "${pkgdir}"/usr/lib/modules/${_kernver}/build

  # now we call depmod...
  depmod -b "${pkgdir}/usr" -F System.map "${_kernver}"

  # sed expression for following substitutions
  local _subst="
    s|%PKGBASE%|${pkgbase}|g
    s|%KERNVER%|${_kernver}|g
    s|%EXTRAMODULES%|${_extramodules}|g
  "

  # install mkinitcpio preset file
  sed "${_subst}" ../linux.preset |
    install -Dm644 /dev/stdin "${pkgdir}/etc/mkinitcpio.d/${pkgbase}.preset"

  # install pacman hooks
#  sed "${_subst}" ../60-linux.hook |
#    install -Dm644 /dev/stdin "${pkgdir}/usr/share/libalpm/hooks/60-${pkgbase}.hook"
#  sed "${_subst}" ../90-linux.hook |
#    install -Dm644 /dev/stdin "${pkgdir}/usr/share/libalpm/hooks/90-${pkgbase}.hook"

  # rather than use another hook (90-linux.hook) rely on mkinitcpio's 90-mkinitcpio-install.hook
  # which avoids a double run of mkinitcpio that can occur
  install -d "${pkgdir}/usr/lib/initcpio/"
  echo "dummy file to trigger mkinitcpio to run" > "${pkgdir}/usr/lib/initcpio/${_kernver}"
}

_package-headers() {
  pkgdesc="Header files and scripts for building modules for linux kernel - ${_desc}"
  provides=("linux-headers=${pkgver}")
  conflicts=('linux-headers')
  replaces=('linux-aarch64-headers')

  cd ${_srcname}
  local _builddir="${pkgdir}/usr/lib/modules/${_kernver}/build"

  install -Dt "${_builddir}" -m644 Makefile .config Module.symvers
  install -Dt "${_builddir}/kernel" -m644 kernel/Makefile

  mkdir "${_builddir}/.tmp_versions"

  cp -t "${_builddir}" -a include scripts

  install -Dt "${_builddir}/arch/${KARCH}" -m644 arch/${KARCH}/Makefile
  install -Dt "${_builddir}/arch/${KARCH}/kernel" -m644 arch/${KARCH}/kernel/asm-offsets.s
  install -Dt "${_builddir}" -m644 vmlinux

  cp -t "${_builddir}/arch/${KARCH}" -a arch/${KARCH}/include
  mkdir -p "${_builddir}/arch/arm"
  cp -t "${_builddir}/arch/arm" -a arch/arm/include

  install -Dt "${_builddir}/drivers/md" -m644 drivers/md/*.h
  install -Dt "${_builddir}/net/mac80211" -m644 net/mac80211/*.h

  # http://bugs.archlinux.org/task/13146
  install -Dt "${_builddir}/drivers/media/i2c" -m644 drivers/media/i2c/msp3400-driver.h

  # http://bugs.archlinux.org/task/20402
  install -Dt "${_builddir}/drivers/media/usb/dvb-usb" -m644 drivers/media/usb/dvb-usb/*.h
  install -Dt "${_builddir}/drivers/media/dvb-frontends" -m644 drivers/media/dvb-frontends/*.h
  install -Dt "${_builddir}/drivers/media/tuners" -m644 drivers/media/tuners/*.h

  # add xfs and shmem for aufs building
  mkdir -p "${_builddir}"/{fs/xfs,mm}

  # copy in Kconfig files
  find . -name Kconfig\* -exec install -Dm644 {} "${_builddir}/{}" \;

  # remove unneeded architectures
  local _arch
  for _arch in "${_builddir}"/arch/*/; do
    [[ ${_arch} == */${KARCH}/ || ${_arch} == */arm/ ]] && continue
    rm -r "${_arch}"
  done

  # remove documentation files
  rm -r "${_builddir}/Documentation"

  # remove now broken symlinks
  find -L "${_builddir}" -type l -printf 'Removing %P\n' -delete

  # strip scripts directory
  local file
  while read -rd '' file; do
    case "$(file -bi "$file")" in
      application/x-sharedlib\;*)      # Libraries (.so)
        strip $STRIP_SHARED "$file" ;;
      application/x-archive\;*)        # Libraries (.a)
        strip $STRIP_STATIC "$file" ;;
      application/x-executable\;*)     # Binaries
        strip $STRIP_BINARIES "$file" ;;
      application/x-pie-executable\;*) # Relocatable binaries
        strip $STRIP_SHARED "$file" ;;
    esac
  done < <(find "${_builddir}" -type f -perm -u+x ! -name vmlinux -print0 2>/dev/null)
  strip $STRIP_STATIC "${_builddir}/vmlinux"
  
  # remove unwanted files
  find ${_builddir} -name '*.orig' -delete
}

pkgname=("${pkgbase}" "${pkgbase}-headers")
for _p in ${pkgname[@]}; do
  eval "package_${_p}() {
    _package${_p#${pkgbase}}
  }"
done
