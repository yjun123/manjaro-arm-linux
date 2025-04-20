# AArch64 multi-platform
# Maintainer: Dan Johansen <strit@manjaro.org>
# Contributor: Kevin Mihelich <kevin@archlinuxarm.org>
# Contributor: Dragan Simic <dsimic@buserror.io>

pkgbase=linux
pkgver=6.14.3
pkgrel=1
_newversion=false
_stopbuild=false    # Will also stop if ${_newversion} is true
_srcname="linux-${pkgver/%.0/}"
_kernelname="${pkgbase#linux}"
_desc="AArch64 multi-platform"
arch=('aarch64')
url="http://www.kernel.org/"
license=('GPL2')
makedepends=('xmlto' 'docbook-xsl' 'kmod' 'inetutils' 'bc' 'git' 'dtc')
options=('!strip')
#source=("https://git.kernel.org/torvalds/t/${_srcname}.tar.gz"
source=("https://cdn.kernel.org/pub/linux/kernel/v6.x/linux-$pkgver.tar.xz"
#0000-sound-soc-dont-use-__free_device_node-in-graph_util_parse_dai.patch
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
0570-arm64-dts-allwinner-h6-Protect-SCP-clock.patch
0571-arm64-dts-allwinner-h6-Add-SCPI-protocol.patch
0572-arm64-dts-allwinner-h6-dtsi-add-sound-node.patch
0573-arm64-dts-allwinner-h6-Fix-Cedrus-IOMMU-again.patch
0574-arm64-dts-allwinner-h6.dtsi-add-ac200-nodes.patch
0575-arm64-dts-allwinner-gs1-fix-eMMC-and-incr-vcpu-limit.patch
0576-arm64-dts-allwinner-tanix-tx6-mini-enable-eth.patch
0577-arm64-dts-allwinner-add-Eeachlink-H6-Mini.patch
0578-arm64-dts-allwinner-tanix-tx6-mini-enable-wifi-cpu-dvfs.patch
0579-arm64-dts-allwinner-enable-audio-gs1.patch
0580-arm64-dts-allwinner-tanix-tx6-enable-wifi-cpu-dvfs.patch
0581-arm64-dts-allwinner-h6-normalize-spdif-card-name.patch
0582-arm64-dts-allwinner-h6-add-deinterlace-node.patch
0583-arm64-dts-allwinner-opi3-enable-ethernet.patch
0584-arm64-dts-allwinner-opi3-fixes.patch
0585-arm64-dts-allwinner-add-Tanix-TX6-A.patch
0586-arm64-dts-allwinner-enable-gpu-opp-multiple-boards.patch
0587-arm64-dts-allwinner-add-orangepi-3-lts.patch
0588-arm64-dtsi-allwinner-rework-cpu-gpu-opp.patch
0600-drivers-h616-wip-add-usb-emac2-support.patch
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
0640-arm64-dts-allwinner-h616.dtsi-add-audio-hdmi-vdec.patch
0641-arm64-dts-allwinner-h616.dtsi-add-ths-cpu-gpu-opp-and-dvfs.patch
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
0728-rockchip-iommu-fixes.patch
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
0802-net-wireless-mm2-fixes-aic8800-sdio-v2024_0327_3561b08f.patch
0803-net-wireless-backport-aic8800-usb-v2024_0327_3561b08f.patch
0804-net-wireless-mm2-fixes-aic8800-usb-v2024_0327_3561b08f.patch
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
1001-math.h-add-DIV_ROUND_UP_NO_OVERFLOW.patch
1002-clk-divider-Fix-divisor-masking-on-64-bit-platforms.patch
1003-clk-composite-replace-open-coded-abs_diff.patch
#1010-FROM-ML-phy-phy-rockchip-samsung-hdptx-Don-t-use-dt-.patch
#1011-FROM-UPSTREAM-drm-rockchip-Don-t-change-hdmi-referen.patch
1012-FROM-UPSTREAM-drm-rockchip-vop2-Drop-unnecessary-if_.patch
1013-FROM-UPSTREAM-drm-rockchip-vop2-Improve-display-mode.patch
1014-WIP-drm-rockchip-vop2-Improve-display-modes-handling.patch
1015-drm-bridge-dw-hdmi-Sync-comments-with-actual-bus-for.patch
1016-drm-bridge-connector-Sync-supported_formats-with-com.patch
1017-drm-connector-hdmi-Evaluate-limited-range-after-comp.patch
1018-drm-connector-hdmi-Add-support-for-YUV420-format-ver.patch
1019-drm-connector-hdmi-Improve-debug-message-for-support.patch
1020-drm-connector-hdmi-Use-YUV420-output-format-as-an-RG.patch
1021-phy-Add-HDMI-configuration-options.patch
1022-phy-hdmi-Add-color-depth-configuration.patch
1023-phy-rockchip-samsung-hdptx-Fix-clock-ratio-setup.patch
1024-phy-rockchip-samsung-hdptx-Drop-unused-lcpll_config.patch
1025-phy-rockchip-samsung-hdptx-Setup-TMDS-char-rate-via-.patch
1026-phy-rockchip-samsung-hdptx-Add-high-color-depth-mana.patch
1027-phy-rockchip-samsung-hdptx-Cleanup-internal-rate-han.patch
1028-phy-rockchip-samsung-hdptx-Avoid-Hz-hHz-unit-convers.patch
1029-TEST-phy-rockchip-samsung-hdptx-Add-verbose-logging.patch
1030-WIP-drm-bridge-Add-detect_ctx-hook.patch
1031-WIP-drm-bridge-connector-Switch-from-detect-to-detec.patch
1032-WIP-drm-bridge-dw-hdmi-qp-Add-high-TMDS-clock-ratio-.patch
1033-WIP-drm-rockchip-vop2-Add-high-color-depth-support.patch
1034-WIP-drm-rockchip-vop2-Add-YUV420-support.patch
1035-WIP-drm-rockchip-dw_hdmi_qp-Make-use-of-phy_configur.patch
1036-WIP-drm-rockchip-dw_hdmi_qp-Add-10bpc-and-YUV420-out.patch
1037-WIP-drm-bridge-dw-hdmi-qp-Enable-10bpc-and-YUV420.patch
1038-FROM-ML-clk-check-for-disabled-clock-provider.patch
1040-drm-bridge-synopsys-add-audio-support-for-dw-hdmi-qp-v7.patch
1045-drm-bridge-synopsys-add-cec-support.patch
1047-drm-rockchip-rk3588-add-edp-support-v6.patch
1048-phy-rockchip-samsung-hdptx-add-edp-mode-support-v7.patch
1049-drm-bridge-synopsys-add-dw-dptx-controller-support-library-v2.patch
1050-drm-rockchip-add-rk3588-dptx-output-support-v2.patch
1051-drm-rockchip-vop2-fix-copy-erro-affecting-dp1-usage.patch
1052-phy-rockchip-usbdp-only-verify-link-voltage-when-flags-are-set.patch
1053-phy-rockchip-usbdp-avoid-call-hpd_event_trigger-in-dp_phy_init.patch
1060-net-ethernet-add-yt6801-gige-pcie-controller.patch
1061-net-ethernet-yt6801-gige-pcie-silence-debug-msgs.patch
1062-WIP-iommu-rockchip-add-flush_iotlb_all-ops.patch
1063-media-rockchip-add-rkvdec2-driver.patch
1064-media-rkvdec2-add-iommu-support-v3.patch
1065-wip-add-hevc-support.patch
1066-wip-hevc-add-ref-frames-support.patch
#1067-wip-rkvdec2-fix-iommu.patch
1067-wip-rkvdec2-fix-iommu-v2.patch
#1068-wip-hevc-remove-rps-support.patch
1070-arm64-dtsi-rk3588s-add-vop2-clock-resets.patch
1071-arm64-dtsi-rockchip-3588s-add-hdmi-bridge.patch
1072-arm64-dtsi-rockchip-3588-hdmi-add-audio-support.patch
1073-arm64-dtsi-rockchip-add-rkvdec2-video-vecoder-on-rk3588.patch
1074-arm64-dtsi-rkvdec2-add-iommu-support-v3.patch
1075-arm64-dtsi-rockchip-rk356x-add-rkvdec2-video-decoder-nodes.patch
1076-arm64-dtsi-rockchip-add-dw-dp-nodes.patch
1077-arm64-dtsi-rockchip-add-samsung-edp-nodes.patch
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
1100-clk-sunxi-ng-add-A523-clock-support.patch
1101-pinctrl-sunxi-Add-support-for-the-Allwinner-A523.patch
1123-dt-bindings-mmc-sunxi-Simplify-compatible-string-lis.patch
1124-dt-bindings-mmc-sunxi-add-compatible-strings-for-All.patch
1125-dt-bindings-watchdog-sunxi-add-Allwinner-A523-compat.patch
1126-watchdog-sunxi_wdt-Add-support-for-Allwinner-A523.patch
1127-dt-bindings-irq-sun7i-nmi-document-the-Allwinner-A52.patch
#1128-irqchip-sunxi-nmi-Support-Allwinner-A523-NMI-control.patch
1129-dt-bindings-phy-document-Allwinner-A523-USB-2.0-PHY.patch
1131-dt-bindings-vendor-prefixes-Add-YuzukiHD-name.patch
1132-dt-bindings-arm-sunxi-Add-new-board-names-for-A523-g.patch
1136-dt-bindings-arm-sunxi-Add-YuzukiHD-Chameleon-board-n.patch
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
1200-dt-bindings-add-rk3528-clock-reset-definitions.patch
1201-clk-rockchip-add-clock-controller-for-the-RK3528.patch
1202-pinctrl-rockchip-add-rk3528-support.patch
1203-dt-bindings-power-add-RK3528-SoCs-header-for-idle.patch
1204-ethernet-stmmac-dwmac-rk3528-add-GMAC-support.patch
1205-soc-rockchip-power-domain-add-rk3528-support.patch
1206-phy-rockchip-inno-usb2-add-phy-support-for-rk3528.patch
1208-thermal-rockchip-add-support-for-rk3528.patch
1209-phy-rockchip-naneng-combphy-add-support-for-rk3528.patch
1210-phy-rockchip-inno-hdmi-add-support-for-rk3528.patch
1211-drm-rockchip-dw_hdmi-add-support-for-rk3528.patch
1213-nvmem-rockchip-otp-add-support-for-rk3528.patch
1214-sound-soc-codecs-add-rk3528-support.patch
1215-hack-hack-gpu-drm-rockchip-rockchip_vop2_reg-add-rk3528.patch
1250-arm64-dtsi-rockchip-add-3528.dtsi.patch
1251-arm64-dts-rockchip-add-dts-for-vontar_r3.patch
1252-arm64-dts-rockchip-rk3528-add-dts-for-rock2a-rock2f.patch
	config
        linux.preset)
#        60-linux.hook
#        90-linux.hook)

md5sums=('fa7f4ad7ad3e48476b6fe3f282fabf2c'
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
         'fac6a4de3708bb8a2423a12a592120bb'
         '554fd010bfcfd195deeaaa5a180499b9'
         'cb47353acc35d5ef90d2c4a1f51ef6e1'
         'ff3e22baa0060cbc6b8d7956b166680e'
         'aa19151df8770f0fa126a93fade5d115'
         '428d69fd2f4fcb96af7c5a9aad9af780'
         '1d11d026d9644bc7c9bf8a13c39f4362'
         '638b58066a16da62c6eee019e7db5803'
         'd90fe549764b44cdc542290f5d5cb080'
         '2d31c924cee504820c08c9b08b10e0af'
         '0c6f8d51d8d9f2b0d2ac9fe09acf1a66'
         'd02ce5bb9d708eefb4fb3120d27c681a'
         'e2bf8a4a8706706ef53879c6e0238db4'
         '2e37e312337cb16fc57d5b782f26098b'
         '5259409dc93c0806efc5a7cfaf79f3e6'
         '0b6d168d526c86fae23a0e5ad60aeaf9'
         '0f9f0572d73d09e262a8684d1cb7972a'
         '97b02760dd91244d39094574d8256750'
         '12cea7e2a3e7f6882976440e1bb504af'
         'f443813381896cb685b0012b1d7108d4'
         '42db2fae3d4fc7435de7f756d12d456c'
         '63e44cc95a8b2ede6a5f8ee830e795bc'
         '226ff38d2a1ead67c4457210b2f8f42f'
         '590861813b731c3783645007146b0d09'
         '1fe341d4300e1045927b3c755676f35d'
         '75fdc48ab706cbde4d663807dfe4928c'
         'a36846f6e57848bd58065aaf55c32c23'
         'd8a4addcc3d57f66d48aa61f168c4ee3'
         'a60e60823753eb54c85af4214c9cb104'
         'f68f47d2728f964b399f5ee302f4aaeb'
         'cdad029e1ba91f4182efd3f4d7b1aa89'
         '5ee50f81c91e37c7ebab799b6be333dc'
         'bc9a23ea0127cd757f2d0bc7f8f2c0bf'
         '54e9c55d7a90f00f6a6fc6d2494db9ed'
         'abe67e12862f6aab45af666d27a689ae'
         '2322b63bd374e80189211273b5e21785'
         '0bec4e3a7f3cc36da11e647b2e92330d'
         'afb7fdc35fb492c5b32b229025faff29'
         'a7bee1cf23fb624052eeb43361c20381'
         'bb1dc5da8fa5a1cdc685a0cc2e0d883f'
         '4b820f69ab2b8c22d65498791b6a3ad8'
         '8ba482f313154a54b2eeae6dff0bf5bb'
         '412daf6cf952332ac807409f7cc233d1'
         '39238cbc1d966de98c0978f4287921ad'
         'cbfa0efa5b123208b70986ed10043167'
         '86cb576c046dfa602cbcf5d2eae6af40'
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
         '340440939d477e453e465a2733c4f0a9'
         'fef1c76e0dc928e14f3a84427f33f6ac'
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
         '8f6beb529dc7894fa3cd0915c53a8338'
         'c3620d90472476c7991fc81839a5e390'
         'b101bb9062e3136d1e50afbcecdd657d'
         'cd04c89fd8ddac352942e966d0ae7b24'
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
         '9b956f7aec0ab9caeaa61916a740dcba'
         '85dac6a15f92e16bee8ca7d5b310289f'
         'e41d58ab7198267e35a13267b6271517'
         '2943defe5245062803685ae92aa29481'
         'd209924aaf6138a214582a49a0559623'
         '7473d6f6c53c89ba7005e70f1952d88a'
         '36bf4e41d5557a6651c5ad9e897910ac'
         '3bebcd15ea626db6fb8e09f3077d66dc'
         '477e48f4ba526e58f52925b4db6d46aa'
         'a03ae0f5354bde93c197d4ab5fbe3498'
         'dc27e84f28cc0dc6a4e01de98e8e1415'
         '65ef11d0d59d74eb3caf907420d54f63'
         'f14d28d7d5ce14d8d912ed9d6e5c6a44'
         '258f1bf4aaa7e88d21e04d2e5fc6a50f'
         '60d11d861863b5245115c6f8d82e0845'
         '9b036b19483da9c1dae007382d64e23e'
         '226847fe8c9a4e8f8c49990505d32014'
         '1367f8b0d7713f9e475f7127f90f3e50'
         '0e14eb6034a1c2a3b998b2efcf893301'
         '3516cf12b8d7565677bdcf8e861827ed'
         '967fdb2c333f773082e29d42dfdedeb8'
         '365d51d29db3b2777d327195e2e8e00b'
         '93524d3d144a35844461a5f7bfdac081'
         '81810a31b89d1e3ebe3a002069ccef57'
         '7bc397b0def5f457a52abeb75c8a670e'
         '291528a011769adc7752e3599af7190c'
         'fd5bbd01bfc038a6c09bfa7622d951da'
         'c5c88f69e293769c0fbb929d4ff4683c'
         '1b7e7c8a716cb7f0835253409ee2a7f3'
         '47802e1f836d19751b722719807e66be'
         'ee2cbd5412a97f696e3a1440caa9e2fa'
         '85a40e7b98addf0f7499de367fc6518f'
         'f2498ecfdbe083a980b91e51c48d22c5'
         'c188a6641f147c52838c034bb12c2c44'
         'da0da81c9fcc4b6465f1cbb11f90a842'
         '6daf2b1c1692847b49bea92d652c9fe2'
         'a0289b7c14990b85711037474fdf8379'
         'b197cbbd6e010d7e681099ee2a52135e'
         'ce15b37780703f2dea9eff82949b0718'
         '7d653321ae7f79d08bbd58e4ac1def0b'
         '3502eb8a17aacac3df37c941461162f8'
         '8f0c414aa221b660f0bfd8c33452c04b'
         '8535559c012b0acfb92a3af9d1739d3f'
         '3aa15bccb1a46204c00c97c495ce7e66'
         'd060cc4b40e501349cfbd4e1a526efe2'
         'a3daeffd6291c149ee148eb7abacc356'
         '3110063dcae53d897161070b63910962'
         '5ad2f4fae8d1e947dd98915eefe0bbe1'
         '0cfc2d453661b5d9d42b2edc871809bb'
         '958a4b71097902f8e4e1289c04f61b7f'
         'ba20191bb8bf68e5c49feb8648e99a61'
         '4e2c1bff5da345de0ff04bf873dd0b4c'
         '6de2a1b7987d89f2b6eeb6e4677a3da0'
         '13c64072621cb9a343f893b733ca1ed6'
         '0ea23db04b96dbf1873c931ad97186f4'
         'e87c97f1ea8d7e099664dce90ba27930'
         'a1af714d915481486f9787451de298b6'
         '27c8f30ef791b188817283ddd74e54a8'
         '8fbeab37cb206009e0b96ef8c462af47'
         'e1c03826ab3db7bb89a873b377b46ef1'
         '9b63b97175f7109a86066dfd45586182'
         'aacf35bf97ee2bb0f2ef81293443aa49'
         '1b23240e3939dab3a05f9a70de2b039a'
         'cafc8d4a33fedfc997f5034c85685f77'
         '2d8abeb75fb7e2887df8adf319d81976'
         'e4eeba7027a8a714719e9bea67681e6b'
         '31604dfb2322699b0d00146744404ef6'
         '29f0d38e99e925d9efefc5d97b224864'
         'adc77295375437d35db99bf01bdb2636'
         '53ccb694389f8b87d33fc3ccb86f6843'
         '9081d7029fc36c8a1a411c2076244b18'
         'a722eb8df102709cba0f49a37c863fb0'
         '1544fd9f0af5d00ad3fb245476cae0e2'
         '47ac799d993db055d5a766ab766d173f'
         '420d406e798d5963773fe96b84307c2c'
         'ee7e6fef3dc0f557069287a4b086f896'
         'c672b634967c195374c80be3fef999f3'
         'fc2aae58f0f5641aab21748d74ff4cf7'
         '494c74c17d54fcd623b7bdd0b4ea2299'
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
         '8b28d597b210e309cfae96febf7487bf'
         '35f3291178707931accc1b167485b64d'
         '54b091b9e12fbd9298c7db2d353a020e'
         '9cf9ef422f300ca98848ca5f0401888b'
         '558ef14a9204a4630207a591dda347a3'
         'b734360131b3b5b028822e345f7e954b'
         '7a94125dedf29fbfd17ccc29699dd1d0'
         'c64719ac0582d3e9f4e633c20703a1e2'
         'bbc75dd2d5a0a15e8efc1b56310051c3'
         '7b90ad2bcb4abefa30851cb535efa5fb'
         '204da62db5e0b7091e9c2e6c5edb282b'
         'e5a9b62f6cced2e2af22b79bb0c49fe9'
         '0f1beb05159edd3ec61e8fec1c0e2b6b'
         '87d01a7d9217c9498e45f5497ccda5cd'
         '8d319a0ae2bbdf1391462a5c58ca6e92'
         '58e6330d9ba69805f910297a946a5e89'
         '0c079c663d450dfd1b82fc0f7105e069'
         '2c938bd8af0dfece71716d879fc71fe0'
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
