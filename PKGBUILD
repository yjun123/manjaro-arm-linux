# AArch64 multi-platform
# Maintainer: Dan Johansen <strit@manjaro.org>
# Contributor: Kevin Mihelich <kevin@archlinuxarm.org>
# Contributor: Dragan Simic <dsimic@buserror.io>

pkgbase=linux
pkgver=6.15.0
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
0520-drm-sun4i-mixer-Add-caching-support.patch
0521-drm-sun4i-dw-hdmi-Deinit-PHY-in-fail-path.patch
0522-drm-sun4i-dw-hdmi-Remove-double-encoder-cleanup.patch
0523-drm-sun4i-dw-hdmi-Switch-to-bridge-functions.patch
0524-drm-sun4i-Don-t-show-error-for-deferred-probes.patch
0525-drm-sun4i-dw-hdmi-Make-sun8i_hdmi_phy_get-more-intui.patch
0526-drm-sun4i-dw-hdmi-check-for-phy-device-first.patch
0527-drm-sun4i-de2-de3-Change-CSC-argument.patch
0528-drm-sun4i-de2-de3-Merge-CSC-functions-into-one.patch
0529-drm-sun4i-de2-de3-call-csc-setup-also-for-UI-layer.patch
0530-drm-bridge-dw-hdmi-add-mtmdsclock-parameter-to-phy-c.patch
0531-drm-bridge-dw-hdmi-support-configuring-phy-for-deep-.patch
0532-drm-sun4i-de3-Add-support-for-YUV420-output.patch
0533-drm-sun4i-de2-Initialize-layer-fields-earlier.patch
0534-drm-sun4i-de3-Implement-AFBC-support.patch
0535-drm-dw-hdmi-cec-sleep-100ms-on-error.patch
0536-drm-bridge-dw-hdmi-fix-4k60-modes-on-some-tv.patch
0537-drm-bridge-synopsys-Fix-CEC-not-working-after-power.patch
0538-HACK-SW-CEC-implementation-for-H3.patch
0550-HACK-clk-sunxi-ng-unify-parent-for-HDMI-clocks.patch
0552-asoc-sun4i-i2s-WiP-multi-channel.patch
0553-media-cedrus-Don-t-CPU-map-source-buffers.patch
0554-media-Add-NV12-and-P010-AFBC-compressed-formats.patch
0555-media-cedrus-add-format-filtering-based-on-depth-and.patch
#0556-media-cedrus-Implement-AFBC-YUV420-formats-for-H265.patch
0557-media-cedrus-Increase-H6-clock-rate.patch
0560-mmc-sunxi-fix-unusuable-eMMC-on-some-H6-boards-by-di.patch
0561-bluetooth-btrtl-add-hci-ver-rtl8822cs.patch
0562-h6-add-sun50i-di-deinterlace-WiP.patch
#0563-hantro-Add-quirk-for-NV12-NV12_4L4-capture-format.patch
0564-pmdomain-sunxi-add-H6-PRCM-PPU-driver-v2.patch
0570-arm64-dts-allwinner-h6-Protect-SCP-clock.patch
0571-arm64-dts-allwinner-h6-Add-SCPI-protocol.patch
0572-arm64-dts-allwinner-h6-dtsi-add-sound-node.patch
0573-arm64-dts-allwinner-h6-Fix-Cedrus-IOMMU-again.patch
0574-arm64-dts-allwinner-h6.dtsi-add-ac200-nodes.patch
0575-arm64-dts-allwinner-gs1-fixes.patch
0576-arm64-dts-allwinner-tanix-tx6-dtsi-fixes.patch
0577-arm64-dts-allwinner-add-Eeachlink-H6-Mini.patch
0578-arm64-dts-allwinner-tanix-tx6-mini-add-eth-wifi.patch
0579-arm64-dts-allwinner-tanix-tx6-add-eth-wifi-vfd.patch
0580-arm64-dts-allwinner-opi3-fixes.patch
0581-arm64-dts-allwinner-add-tanix-tx6-a.patch
0582-arm64-dts-allwinner-h6-add-deinterlace-node.patch
0583-arm64-dts-allwinner-add-orangepi-3-lts.patch
#0600-drivers-h616-wip-add-usb-emac2-support.patch
0601-drivers-thermal-allwinner-add-h616-ths-support.patch
0602-media-cedrus-add-H616-variant.patch
0603-soc-sunxi-sram-Add-SRAM-C1-H616-handling.patch
0604-dma-sun6i-dma-add-h616-support.patch
0610-drivers-drm-wip-add-h616-hdmi.patch
0615-drivers-iommu-sun50i-iommu-fix-iommu-on-h616.patch
0620-sound-soc-sunxi-add-codec-driver-for-h616.patch
0621-sound-soc-add-sunxi_v2-for-h616-ahub.patch
0623-sound-soc-sunxi-hack-to-fix-oops-on-cards-caps-query.patch
#0630-net-wireless-add-uwe5622-support-v20231020.patch
0631-clk-sunxi-ng-ccu-sun6i-rtc-fix-32k-clk.patch
0632-clk-sunxi-ng-ccu-hack-fix-too-slow-hdmi-audio.patch
0633-regulator-add-mmc-high-speed-SD-UHS-modes-support.patch
0635-drvers-of-add-dt-overlay-configfs-interface.patch
0637-drm-panfrost-enable-G31-on-H616.patch
0640-arm64-dts-allwinner-h616.dtsi-add-audio-hdmi-vdec.patch
0641-arm64-dts-allwinner-h616.dtsi-add-dvfs-and-h313-cpu-opp.patch
0641-arm64-dts-allwinner-h616.dtsi-add-gpu-nodes.patch
0642-arm64-dts-allwinner-h616.dtsi-add-emac1.patch
0643-arm64-dts-allwinner-h616.dtsi-fix-x96q-failing-mmc3.patch
0644-arm64-dts-allwinner-h616-OrangePI-Zero23-enable-ths-hdmi-audio.patch
0645-arm64-dts-allwinner-h616-add-Tanix-TX6s-TVbox.patch
0646-arm64-dts-allwinner-h616-add-Tanix-TX6s-axp313-TVbox.patch
0647-arm64-dts-allwinner-h313-add-x96q-TVbox.patch
0648-arm64-dts-allwinner-h313-add-x96q-lpddr3-TVbox.patch
0649-arm64-dts-allwinner-h618-add-vontar-h618-TVbox.patch
0650-arm64-dts-allwinner-h618-add-opi-2w.patch
0651-arm64-dts-allwinner-h313-Tanix-TX1-TVbox.patch
0652-arm64-dts-allwinner-h313-add-x96q-v5.1-TVbox.patch
0653-arm64-dts-allwinner-h616-add-pendoo-x12pro-tvbox.patch
0654-arm64-dts-allwinner-h618-improve-transpeed-8k618-tvbox.patch
0655-arm64-dts-allwinner-h313-h616-h618-add-cpu-overclock-via-overlays.patch
0656-arm64-dts-allwinner-h313-h616-h618-add-gpu-overclock-via-overlays.patch
0703-media-v4l2-common-Add-helpers-to-calculate-bytesperl.patch
0704-media-v4l2-Add-NV15-and-NV20-pixel-formats.patch
0705-media-rkvdec-h264-Use-bytesperline-and-buffer-height.patch
0706-media-rkvdec-h264-Don-t-hardcode-SPS-PPS-parameters.patch
0707-media-rkvdec-Extract-rkvdec_fill_decoded_pixfmt-into.patch
0708-media-rkvdec-Move-rkvdec_reset_decoded_fmt-helper.patch
0709-media-rkvdec-Extract-decoded-format-enumeration-into.patch
0710-media-rkvdec-Add-image-format-concept.patch
0711-media-rkvdec-Add-get_image_fmt-ops.patch
0712-media-rkvdec-h264-Support-High-10-and-4-2-2-profiles.patch
0714-media-rkvdec-Add-HEVC-backend.patch
0715-media-rkvdec-Add-variants-support.patch
0716-media-rkvdec-Implement-capability-filtering.patch
0717-media-rkvdec-Add-RK3288-variant.patch
0718-media-rkvdec-Disable-QoS-for-HEVC-and-VP9-on-RK3328.patch
0722-v4l2-wip-iep-driver.patch
0724-media-rkvdec-add-soft-reset-on-errors.patch
0725-drm-rockchip-vop-add-immutable-zpos-property-fix-z-order.patch
0727-drm-rockchip-vop2-rk356x-reorder-wins-fix-osd-in-drm-planes.patch
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
0800-Enable-rk356x-PCIe-controller.patch
0801-net-wireless-backport-aic8800-sdio-v2024_0327_3561b08f.patch
0803-net-wireless-backport-aic8800-usb-v2024_0327_3561b08f.patch
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
#0905-drivers-add-rpi5-clk-pinctrl-mmc-pwm-net-usb-pci-rp1.patch
#0906-gpu-drm-vc4-add-rpi5-support.patch
#0950-arm64-dts-brcm-set-userled-to-mmc.patch
#0951-arm64-dts-brcm-add-rpi5-dt.patch
#0953-arm64-dts-add-rpivid-rpi4.patch
1003-math.h-add-DIV_ROUND_UP_NO_OVERFLOW.patch
1004-clk-divider-Fix-divisor-masking-on-64-bit-platforms.patch
1005-clk-composite-replace-open-coded-abs_diff.patch
1015-mfd-rk8xx-Fix-shutdown-handler.patch
1016-dt-bindings-display-vop2-Add-VP-clock-resets.patch
1017-drm-rockchip-vop2-Add-clock-resets-support.patch
1022-drm-rockchip-vop2-Add-core-reset-support.patch
1025-phy-Add-HDMI-configuration-options.patch
1026-phy-hdmi-Add-color-depth-configuration.patch
1027-phy-rockchip-samsung-hdptx-Fix-clock-ratio-setup.patch
1028-phy-rockchip-samsung-hdptx-Do-no-set-rk_hdptx_phy-ra.patch
1029-phy-rockchip-samsung-hdptx-Drop-unused-struct-lcpll_.patch
1030-phy-rockchip-samsung-hdptx-Drop-unused-phy_cfg-drive.patch
1031-phy-rockchip-samsung-hdptx-Drop-superfluous-cfgs-dri.patch
1032-phy-rockchip-samsung-hdptx-Avoid-Hz-hHz-unit-convers.patch
1033-phy-rockchip-samsung-hdptx-Setup-TMDS-char-rate-via-.patch
1034-phy-rockchip-samsung-hdptx-Provide-config-params-val.patch
1035-phy-rockchip-samsung-hdptx-Restrict-altering-TMDS-ch.patch
1036-phy-rockchip-samsung-hdptx-Rename-ambiguous-rk_hdptx.patch
1037-phy-rockchip-samsung-hdptx-Optimize-internal-rate-ha.patch
1038-phy-rockchip-samsung-hdptx-Add-high-color-depth-mana.patch
1039-WIP-drm-rockchip-dw_hdmi_qp-Make-use-of-phy_configur.patch
1040-WIP-drm-bridge-Add-detect_ctx-hook.patch
1041-WIP-drm-bridge-connector-Switch-from-detect-to-detec.patch
1042-WIP-drm-bridge-dw-hdmi-qp-Add-high-TMDS-clock-ratio-.patch
1043-drm-dp-Pull-drm_dp_link_power_up-down-from-Tegra-to-.patch
1044-drm-bridge-cdns-mhdp8546-Switch-to-common-helpers-to.patch
1045-drm-bridge-anx6345-Switch-to-common-helpers-to-power.patch
1046-drm-bridge-anx78xx-Switch-to-common-helpers-to-power.patch
1047-drm-bridge-it6505-Switch-to-common-helpers-to-power-.patch
1049-dt-bindings-display-rockchip-Add-schema-for-RK3588-D.patch
1050-drm-bridge-synopsys-Add-DW-DPTX-Controller-support-l.patch
1051-drm-rockchip-Add-RK3588-DPTX-output-support.patch
1052-dt-bindings-display-simple-bridge-Add-ra620-compatib.patch
1053-drm-birdge-simple-bridge-Add-support-for-radxa-ra620.patch
1054-media-v4l2-ctrls-core-Set-frame_mbs_only_flag-by-def.patch
1055-media-rockchip-Move-H264-CABAC-table-to-header-file.patch
1056-media-rockchip-Introduce-the-rkvdec2-driver.patch
1057-media-dt-bindings-rockchip-Document-RK3588-Video-Dec.patch
1058-drm-bridge-synopsys-add-cec-support.patch
1060-net-ethernet-add-yt6801-gige-pcie-controller.patch
1061-net-ethernet-yt6801-gige-pcie-silence-debug-msgs.patch
1062-WIP-iommu-rockchip-add-flush_iotlb_all-ops.patch
1064-media-rkvdec2-add-iommu-support-v3.patch
1065-wip-add-hevc-support.patch
1066-wip-hevc-add-ref-frames-support.patch
1067-wip-rkvdec2-fix-iommu-v2.patch
1068-dt-bindings-PCI-dw-rockchip-Add-rk3576-support.patch
#1068-wip-hevc-remove-rps-support.patch
1070-arm64-dtsi-rk3588s-add-vop2-clock-resets.patch
1073-arm64-dtsi-rockchip-add-rkvdec2-video-vecoder-on-rk3588.patch
1074-arm64-dtsi-rkvdec2-add-iommu-support-v3.patch
1075-arm64-dtsi-rockchip-rk356x-add-rkvdec2-video-decoder-nodes.patch
1076-arm64-dtsi-rockchip-add-dw-dp-nodes.patch
1080-arm64-dts-rockchip-rk3588s-rock5a-dts-improvements.patch
1081-arm64-dts-rockchip-rk3588-rock5b-dts-improvements.patch
1082-arm64-dts-rockchip-rk3588s-rock5c-dts-improvements.patch
1083-arm64-dts-rockchip-rk3588-rock5itx-dts-improvements.patch
1084-arm64-dts-rockchip-rk3588s-opi5-dts-improvements.patch
1085-arm64-dts-rockchip-rk3588-opi5plus-dts-improvements.patch
1086-arm64-dts-rockchip-rk3588s-add-opi5pro-dts.patch
1087-arm64-dts-rockchip-rk3588s-add-nanopi-m6-dts.patch
1088-arm64-dts-rockchip-rk3588s-nanopc-r6s-dts-improvements.patch
1089-arm64-dts-rockchip-rk3588-nanopc-t6-dtsi-improvements.patch
1090-arm64-dts-rockchip-rk3588-add-rock5t-dt.patch
1139-net-ethernet-allwinner-add-gmac200-support.patch
1140-net-ethernet-allwinner-add-gmac-support.patch
1141-thermal-drivers-sun8i-add-initial-support-for-ths-v2.patch
1142-add-initial-cpufreq-support.patch
1150-arm64-dtsi-allwinner-add-initial-A523-support.patch
1151-arm64-dtsi-allwinner-add-gmac1-in-A523-dtsi.patch
1152-arm64-dtsi-allwinner-add-gmac0-in-A523-dtsi.patch
1153-arm64-dtsi-allwinner-add-ths-support-v2.patch
1154-arm64-dtsi-allwinner-add-cpufreq-support.patch
1170-arm64-dts-allwinner-h728-add-x96q-pro-tvbox-plus.patch
1172-arm64-dts-allwinner-t527-add-orangepi-4a-dts.patch
1173-arm64-dts-allwinner-a527-add-Radxa-A5E-support.patch
	config
        linux.preset)
#        60-linux.hook
#        90-linux.hook)

md5sums=('f37783334d33320667a67d8b3c343299'
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
         'ee87f7f93441497058fb3ebbc386a2c1'
         '852eae6e396daac53bc4a32693fd9647'
         '2d8e3a65a196bab6dec559a1d8010d21'
         '320b62f13387f4db0b154a582eacdc70'
         '294c3f250b5afa17f57e79944c4d529f'
         'd28b7ed9ab5ffb4080d2ab07caac26b9'
         '2f28d6a7ee59fd6b4693346a9df93beb'
         '461b9f84cf0daea89f1bdbfba27b0279'
         'cfc48c553aab7fdf43ce1f288d7d7b33'
         '67633bce93c27a2f264a17373dd5b32a'
         '1f1d8ae4ede5f0679310b65076749a2e'
         'c3e9d498c6b413e157433d6a509a81b4'
         '046df9d0731dc40f24406fe01626680b'
         '16bdd52da169cf36ed6908043cc94eb6'
         '69d20cb387d4de8dfcdfef0a7cb6e4e6'
         '7377e24f367aefded32626d68036637f'
         'e4a4657990a54cdc00f8ecb322aa6049'
         '630efe044f9ec1d3a7c4cc6a15c4219a'
         '612ff6468c9ab2ea6d6d91a14de7f31a'
         '8488af1e862c67cf7e41753b96aeea6b'
         '1699b20e867741a86c35d743b4a17df4'
         '95b517e62538ac03f522e8a5b3660fb8'
         '874b8b9b17ffd156d4f0dfa4b1a5e81e'
         '39790f191e61387817480a50899600a9'
         '4f0853228839336c69adcb2d9dadf2b3'
         '0e6ebee7a6c045dd7cf45cbafbf924bb'
         '1dcafc57cdbc3421e12ab54a54c8284c'
         'f912776f05276c66311105f57fb5d475'
         '9caaf988520667da09769f58933193d4'
         'fac6a4de3708bb8a2423a12a592120bb'
         '554fd010bfcfd195deeaaa5a180499b9'
         'cb47353acc35d5ef90d2c4a1f51ef6e1'
         'ff3e22baa0060cbc6b8d7956b166680e'
         'aa19151df8770f0fa126a93fade5d115'
         '2311d1b0063b0ecbb222fa1449872891'
         '9a2723bd97b748eb7507b8971d02aee6'
         '2a8daf86328b8ae4e7fb875652dc19d2'
         '07b3e3979d7f5e85e37182574b8efe89'
         'f800aa07f46e08fd39a5996fc00c4ae7'
         'e3a0b0484fd17975620289818fc9c885'
         'd5b94392123677bb62106f9a25484b04'
         'e2bf8a4a8706706ef53879c6e0238db4'
         '97b02760dd91244d39094574d8256750'
         '42db2fae3d4fc7435de7f756d12d456c'
         '63e44cc95a8b2ede6a5f8ee830e795bc'
         '226ff38d2a1ead67c4457210b2f8f42f'
         '590861813b731c3783645007146b0d09'
         '1fe341d4300e1045927b3c755676f35d'
         '75fdc48ab706cbde4d663807dfe4928c'
         'a36846f6e57848bd58065aaf55c32c23'
         '2b5ffe71dd9b653df00d04819c71ac25'
         'a60e60823753eb54c85af4214c9cb104'
         'f68f47d2728f964b399f5ee302f4aaeb'
         'cdad029e1ba91f4182efd3f4d7b1aa89'
         '5ee50f81c91e37c7ebab799b6be333dc'
         '4257bf04a0e285d6caeb4a3e1519226f'
         '733ce6d60ef14abdd7b9f595070d818a'
         'c5eb21b3b6f59b2a37d2cc4c8f68701f'
         'f6b66e3e5ea6529ee335a432ad008b21'
         '9f29dc701e0419c71ef3ae865bc38a96'
         'abe67e12862f6aab45af666d27a689ae'
         '2322b63bd374e80189211273b5e21785'
         '0bec4e3a7f3cc36da11e647b2e92330d'
         'f9998f900ecf9adf591458350c1cb4c1'
         '8ea4e897daf72e5d340b8ae871ea579c'
         'e2aa6c05e27f4604a1c8c94fb06ab3c1'
         '6fc13c55b4815b115364654e14c5d1aa'
         'cabb2016cd42344f65478ac4ee0d3413'
         '412daf6cf952332ac807409f7cc233d1'
         '35247f091a92cd6b298ff7b40d0f789b'
         '13590c1735d08b141c077f149f1ec4bb'
         'dae7b7e510c1b05c17e0ae9a1ee45e6e'
         '8a387289e6084ea76da96b30fd02ec0e'
         'df6a260763dafb5e6757bbb885ed1bed'
         'a06129a8cf6a487e65af60c85aacb5ab'
         '637985e20b9cf4fcf626dbca9dfd2935'
         'c7f1d6191f815be44437b9586d8f8aec'
         '32e8556d1a85cabb1029fa65f780a85d'
         '807fabeeb5ebe42ab7b65ed9db1863bf'
         '3f437e26c040c79d66236a8e0402f7a2'
         'a49d9972d38cd1606fd22958a170a698'
         '8a5484a2d42d41ce2b2bd0042826f620'
         'de5265485a8ad360187d103a8719905f'
         '814ce314ff15be52f1f25bb9c8cbd3da'
         '67878818a815d55747de1a972ad90ea7'
         '4abc87044c9f2e381fb2c4194e86ac99'
         '45bc395f9e0b23211fcb9077fccac1c5'
         '9183deade6c26c8008b0ab72ab26566e'
         '536d5d5b90abd1c28ac22c8c2d82601f'
         'ab44f24c639034d099dbb0d0b39f0d49'
         '031646e4ddde55979488a7c9f44fe76d'
         'a59e2731f8f9b78ecb11fc2fbc7251f7'
         'e7ae0a54c830f35a9eb41f8db035fc68'
         '0db550634152688fc7211e055dfa2129'
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
         '36f183da40a11eaf6245b12aa0092684'
         'd09d628295c8427bd9b30552f687ecd4'
         '838c036f502bb251fba7ebf098fd3ac4'
         'ca782317804d7eca9aad74f2dcdc12a0'
         'e87f12a7315571bdb20092be976dea69'
         'aa82f20d5d6ec8affc6915058c2d4ab2'
         'd559a352374a2becd9fb6d30c6c7b6cf'
         '6b514cb03ef096d5d2f42a8b4332d918'
         '94a9317c40a68c10504f492a0abf72da'
         '7ff3b7e09aaefa3060fb18a6bc04d367'
         '0f38739e23894da7251ee14e35bed22b'
         'f556b3ac831a63f35aada54df93d40ea'
         '9a325a4e8febfdd8b13b3713be3a30a4'
         '48c85cf2e1b0df6bd0f8c73525e1d999'
         '8979801afff6e1407ecb61d7a7de8652'
         'a2e0c1f541044bdf845dc85182bdd685'
         '59fa47be5f410dc12516b03a7212b0e4'
         'f06731cfb7b2812d6d4d125d13ceca70'
         'fc4908203b9799983494bcfb7db0503e'
         '6425b1cb85e02afb1d901fba7ce67316'
         '8fd57b490ce42f7e92bbd5c170133185'
         '13d55b469c784a5aec977a3578377852'
         '9fe4b5a243141e12b7e34a8e13b56148'
         '4c3db6c8543c297d751b57755bbcc569'
         '637b92ef203016df9a22878dcd2c4f63'
         '2970d36cded0482ad91611c482b58884'
         '0c8128b3b39ad39a6f0d1811c0e543d5'
         'ca4b874d1e52af6b9af83d28a33e184e'
         '6ddc357448834dfbc8224b0aa1e168f6'
         'f26675e9ccf4dc48a5fd938a9f4ab366'
         '974fbea11bfa184b8576d6f642ac8b64'
         'ece2375f9e31807b0ca2141337695fdb'
         'e4ef07555407e9497d887ee29b4816b0'
         '1b3c1be63d4e4bd22b4545871bfd85b7'
         'ccde1c9b35640bfd2cb62190ddc21019'
         '0467455e59158aa0a8167cb0772f238b'
         '18c40cc3badb07b52606c78dd859a12a'
         'b25d1f2ff5a2614771b0fc1960827239'
         '8d6c800c8c24bb8c5db5f2cdd35d9ce0'
         '303760696acf1f674d663b7d19e5ae15'
         '4a43851b350aa5838c3a9d2062759625'
         '2a662945082e1c33c70cc133497b70f8'
         'f765d7d009139f535cff6c3d12f6a45f'
         '021bba653bd155b089e71f06410064f4'
         '0c781a51fad7c06b0cf56f76448cca28'
         '58e98fe49f27f23bc0e567afe455baf9'
         '0f71317a2a6d6e400f1d6e2a828f0072'
         '524859aa28f1e070fe5d1f14baaa4e8f'
         '82f519d53438e9cde3d809893353988c'
         'f29db24d419d7eef14ac86afc068732f'
         'd61e30794d7476635ab1c737f2945f60'
         '5e8b415174ba6186f8412142d2234b6f'
         '1b4d45f6a0a6d2e6e6fbd88885a05b43'
         'cf2063317eac8792e1f7ac1c5bf84a82'
         '20a8c0b0db6a4e9b74ac8d5c8e8e840a'
         '0c254aad39c67e8a714f9971556679a6'
         '85a40e7b98addf0f7499de367fc6518f'
         '7d653321ae7f79d08bbd58e4ac1def0b'
         '3502eb8a17aacac3df37c941461162f8'
         '8f0c414aa221b660f0bfd8c33452c04b'
         '3aa15bccb1a46204c00c97c495ce7e66'
         'd060cc4b40e501349cfbd4e1a526efe2'
         'a3daeffd6291c149ee148eb7abacc356'
         '3110063dcae53d897161070b63910962'
         'baf610b7496daf4737838ea704608c5e'
         '5ad2f4fae8d1e947dd98915eefe0bbe1'
         'ba20191bb8bf68e5c49feb8648e99a61'
         '4ab61a2a4976138ab63a23627c0d7a98'
         '6de2a1b7987d89f2b6eeb6e4677a3da0'
         '13c64072621cb9a343f893b733ca1ed6'
         'e87c97f1ea8d7e099664dce90ba27930'
         '4aeb7369025cc001e5244f7686431fc3'
         '93531742c48d4712912a9504dd605c85'
         '24f6572dee7852113df332756b22d7cc'
         'e1c03826ab3db7bb89a873b377b46ef1'
         '009204babeb051c758aaeeefacea0fe1'
         '4be073f2f73e5a6e5b3dedfc5dce1d4a'
         '097d9c47a265d9cb96e06751101c50e1'
         'cafc8d4a33fedfc997f5034c85685f77'
         '2d8abeb75fb7e2887df8adf319d81976'
         'd0761cb38080b6a2eedfe0627b90aebb'
         '2861570a42260aefeca3f47068790770'
         '0241de0ab1510cbc576ed2d3b37216bf'
         '11ef441b24bf9eb61096a501e1770610'
         '303c9d173d254b13417763c1c1697f08'
         '13efef565f5a8d47a5246acae9e6d7de'
         '6dcab0586d2dd7025502f6edbba07be6'
         'ef7951f77136006c01f878a02d418e19'
         '78ed0608a68f6c088ab73cc48becbeac'
         'dfc0a51a332c23d6ef41db60268ce5ec'
         'bf641fb3d6133507b1bc5420f28c7050'
         'c69b927e7638d1b91ee658fa472f282b'
         'cf0a9682357b5cf9b282e4b78ad9d48a'
         '4b0ec61fe8fac3a92473c358bf1a1a4a'
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
  install -d "${pkgdir}/usr/lib/firmware/"
  echo "dummy file to trigger mkinitcpio to run" > "${pkgdir}/usr/lib/firmware/${_kernver}"
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
