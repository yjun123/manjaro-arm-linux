# AArch64 multi-platform
# Maintainer: Dan Johansen <strit@manjaro.org>
# Contributor: Kevin Mihelich <kevin@archlinuxarm.org>
# Contributor: Dragan Simic <dsimic@buserror.io>

pkgbase=linux
pkgver=6.12.10
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
0556-media-cedrus-Implement-AFBC-YUV420-formats-for-H265.patch
0557-media-cedrus-Increase-H6-clock-rate.patch
0558-media-verisilicon-g2-fix-chroma-offset-calculation.patch
0560-mmc-sunxi-fix-unusuable-eMMC-on-some-H6-boards-by-di.patch
0561-bluetooth-btrtl-add-hci-ver-rtl8822cs.patch
0562-h6-add-sun50i-di-deinterlace-WiP.patch
0563-hantro-Add-quirk-for-NV12-NV12_4L4-capture-format.patch
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
0622-sound-soc-sunxi-add-spdif-spdif.patch
0623-sound-soc-sunxi-hack-to-fix-oops-on-cards-caps-query.patch
0630-net-wireless-add-uwe5622-support-v20231020.patch
0631-clk-sunxi-ng-ccu-sun6i-rtc-fix-32k-clk.patch
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
0750-arm64-dts-rockchip-enable-inno-usb3-beelinkA1-roc-cc.patch
0753-arm64-dts-rockchip-rk3399-radxa-rockpi-bc-remove-wifi-compatible.patch
0754-arm64-dts-rockchip-rk33xx-set-userled-to-mmc.patch
0755-arm64-dts-rockchip-rk3399-add-orangepi-4-and-4-lts.patch
0756-arm64-dts-rockchip-rk33xx-add-eth-wifi-aliases.patch
0757-arm64-dts-rockchip-rk3399-orangepi-4-lts-add-fan-support.patch
0800-Enable-rk356x-PCIe-controller.patch
0801-net-wireless-backport-aic8800-sdio-v2024_0327_3561b08f.patch
0802-net-wireless-mm2-fixes-aic8800-sdio-v2024_0327_3561b08f.patch
0803-net-wireless-backport-aic8800-usb-v2024_0116_ec460377.patch
0804-net-wireless-mm2-fixes-aic8800-usb-v2024_0116_ec460377.patch
0831-arm64-dts-rockchip-enable-usb2-usb3-sata-audio-in-rk35xx.dtsi.patch
0832-arm64-dtsi-rockchip-rk356x-disable-vepu-rga-enable-dfi.patch
0833-arm64-dts-rockchip-enable-Quartz64-A-usb2-usb3-pcie-audio.patch
0834-arm64-dtsi-rockchip-add-missing-reset-names-for-combphy.patch
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
0900-rpi-vc04_services-add_h~l2-m2m_decode-15062024.patch
0901-rpi-vc04_services-bcm2835-codec-remove-isp-formats.patch
0902-media-add-rpivid-driver.patch
0905-drivers-add-rpi5-clk-pinctrl-mmc-pwm-net-usb-pci-rp1.patch
0906-gpu-drm-vc4-add-rpi5-support.patch
0950-arm64-dts-brcm-set-userled-to-mmc.patch
0951-arm64-dts-brcm-add-rpi5-dt.patch
0953-arm64-dts-add-rpivid-rpi4.patch
1008-math.h-add-DIV_ROUND_UP_NO_OVERFLOW.patch
1009-clk-divider-Fix-divisor-masking-on-64-bit-platforms.patch
1010-clk-composite-replace-open-coded-abs_diff.patch
1012-clk-rockchip-handle-missing-clocks-with-EPROBE_DEFER.patch
1013-clk-rockchip-rk3588-register-GATE_LINK-later.patch
1014-clk-rockchip-expose-rockchip_clk_set_lookup.patch
1016-clk-rockchip-implement-linked-gate-clock-support.patch
1017-clk-rockchip-rk3588-drop-RK3588_LINKED_CLK.patch
1018-mfd-rk8xx-Fix-shutdown-handler.patch
1021-WIP-phy-phy-rockchip-samsung-hdptx-Add-FRL-EARC-supp.patch
1022-TESTING-phy-phy-rockchip-samsung-hdptx-Add-verbose-l.patch
1023-vop2-Add-clock-resets-support.patch
1024-WIP-drm-rockchip-vop2-Improve-display-modes-handling.patch
1026-drm-bridge-synopsys-Add-DW-HDMI-QP-TX-controller-dri.patch
1027-drm-rockchip-Add-basic-RK3588-HDMI-output-support.patch
1029-dw-hdmi-qp-Add-missing-capabilities.patch
1030-drm-bridge-synopsys-Fix-HDR-metadata.patch
1031-WIP-Add-a-requested-output-format-proper.patch
1032-WIP-Add-a-min_bpc-hdmi-property.patch
1033-WIP-drm-bridge-synopsys-Add-DW-HDMI-QP-C.patch
1034-debug-patch-from-Andy-Yan.patch
1035-WIP-Add-missing-colorspace-connector-pro.patch
1036-WIP-fix-up-10bpc.patch
1037-drm-rockchip-Set-dma-mask-to-64-bit.patch
1038-drm-rockchip_vop2-add-plane-color-encodi.patch
1039-drm-rockchip-vop2-Fix-cluster-windows-al.patch
1040-drm-rockchip-vop2-Fix-the-mixer-alpha-se.patch
1041-drm-rockchip-vop2-Fix-the-windows-switch.patch
1042-WIP-Support-subsampled-YUV-color-formats.patch
1043-phy-rockchip-samsung-hdptx-dont-use-dt-aliases-to-determine-phy-id.patch.patch
1044-ASoC-rockchip-add-machine-driver-for-hdmi-audio.patch
1045-ASoC-rockchip-hdmi-support-dts-specified-daifmt.patch
1046-ASoC-rockchip-hdmi-Fix-potential-NULL-point-referenc.patch
1047-ASoC-rockchip-i2s-tdm-Add-support-for-Digital-Loopba.patch
1048-ASoC-rockchip-i2s-tdm-Add-support-for-PATHx-controls.patch
1049-drm-bridge-synopsys-Add-audio-support-for-dw-hdmi-qp.patch
1050-drm-rockchip-dw_hdmi-Make-sure-dclk-is-enabled-when-set-audio-regs.patch
1051-phy-rockchip-add-samsung-mipi-dcphy-driver.patch
1052-drm-rockchip-vop2-two-fixes-for-dsi-enablement.patch
1053-drm-rockchip-add-driver-for-the-new-dsi2-controller.patch
1054-phy-rockchip-samsung-hdptx-add-hdmi1-support.patch
1055-drm-bridge-synopsys-dw-hdmi-qp-fix-wrong-cec-clock-v2.patch
1060-net-ethernet-add-yt6801-gige-pcie-controller.patch
1061-net-ethernet-yt6801-gige-pcie-silence-debug-msgs.patch
1062-WIP-iommu-rockchip-add-flush_iotlb_all-ops.patch
1063-media-rockchip-add-rkvdec2-driver.patch
1064-media-rkvdec2-add-iommu-support-v3.patch
1065-wip-add-hevc-support.patch
1066-wip-hevc-add-ref-frames-support.patch
#1067-hack-drm-connector-revert-0485a718f-to-fix-oops-at-boot.patch
1070-arm64-dtsi-rk3588s-add-vop2-clock-resets.patch
1071-arm64-dtsi-rockchip-3588s-add-hdmi0-bridge.patch
1072-arm64-dtsi-rockchip-3588-hdmi-audio-fixup.patch
1074-arm64-dtsi-rockchip-add-rkvdec2-video-vecoder-on-rk3588.patch
1075-arm64-dtsi-rockchip-add-dsi2.patch
1076-arm64-dtsi-rk3588-add-phy-node-for-hdmi1-tx-port.patch
1077-arm64-dtsi-rkvdec2-add-iommu-support-v3.patch
1078-arm64-dtsi-rockchip-rk356x-add-rkvdec2-video-decoder-nodes.patch
1080-arm64-dts-rockchip-rk3588s-rock5a-dts-improvements.patch
1081-arm64-dts-rockchip-rk3588-rock5b-dts-improvements.patch
1082-arm64-dts-rockchip-rk3588-rock5itx-dts-improvements.patch
1083-arm64-dts-add-rock5c-dts.patch
1084-arm64-dts-rockchip-rk3588-opi5plus-dts-improvements.patch
1085-arm64-dts-rockchip-rk3588s-opi5-dts-improvements.patch
1086-arm64-dts-add-opi5pro-dts.patch
1087-arm64-dts-add-nanopi-m6-dts.patch
1088-arm64-dts-rockchip-orangepi-5-plus-Enable-USB-3.0-ports.patch
1089-arm64-dts-add-opi5max-dts.patch
1090-arm64-dts-rockchip-rk3588s-nanopc-r6s-dts-improvements.patch
1091-arm64-dts-rockchip-rk3588-nanopc-t6-dtsi-improvements.patch
1092-arm64-dts-rockchip-rk3588-boards-enable-hdmi1.patch
1101-dt-bindings-mfd-x-powers-axp152-Document-AXP323.patch
1102-mfd-axp20x-ensure-relationship-between-IDs-and-model.patch
1103-mfd-axp20x-Allow-multiple-regulators.patch
1104-mfd-axp20x-Add-support-for-AXP323.patch
1105-regulator-axp20x-add-support-for-the-AXP323.patch
1107-disable-unused-cores-debug.patch
1110-pinctrl-sunxi-refactor-pinctrl-variants-into-flags.patch
1111-pinctrl-sunxi-move-bank-K-register-offset.patch
1112-pinctrl-sunxi-support-moved-power-configuration-regi.patch
1113-pinctrl-sunxi-allow-reading-mux-values-from-DT.patch
1114-dt-bindings-pinctrl-add-compatible-for-Allwinner-A52.patch
1115-pinctrl-sunxi-Add-support-for-the-Allwinner-A523.patch
1116-pinctrl-sunxi-Add-support-for-the-secondary-A523-GPI.patch
1117-clk-sunxi-ng-mp-Add-SUNXI_CCU_P_DATA_WITH_MUX_GATE-w.patch
1118-clk-sunxi-ng-mp-introduce-dual-divider-clock.patch
1119-clk-sunxi-ng-mp-provide-wrapper-for-setting-feature-.patch
1120-dt-bindings-clk-sunxi-ng-add-compatible-for-the-A523.patch
1121-dt-bindings-clk-sunxi-ng-add-compatible-for-the-A523.patch
1122-clk-sunxi-ng-Add-support-for-the-A523-T527-CCU.patch
1123-clk-sunxi-ng-add-support-for-the-A523-T527-PRCM-CCU.patch
1124-dt-bindings-mmc-sunxi-Simplify-compatible-string-lis.patch
1125-dt-bindings-mmc-sunxi-add-compatible-strings-for-All.patch
1126-dt-bindings-watchdog-sunxi-add-Allwinner-A523-compat.patch
1127-watchdog-sunxi_wdt-Add-support-for-Allwinner-A523.patch
1128-dt-bindings-i2c-mv64xxx-Add-Allwinner-A523-compatibl.patch
1129-dt-bindings-irq-sun7i-nmi-document-the-Allwinner-A52.patch
1130-dt-bindings-phy-document-Allwinner-A523-USB-2.0-PHY.patch
1131-dt-bindings-usb-sunxi-musb-add-Allwinner-A523-compat.patch
1132-dt-bindings-usb-add-A523-compatible-string-for-EHCI-.patch
1133-dt-bindings-rtc-sun6i-Add-Allwinner-A523-support.patch
1135-dt-bindings-vendor-prefixes-Add-YuzukiHD-name.patch
1136-dt-bindings-arm-sunxi-Add-Avaota-A1-board.patch
1137-net-phy-add-Maxio-MAE0621A-phy-driver.patch
1138-clk-sunxi-ng-add-support-for-A523-T527-gmac1-clocks.patch
1139-net-ethernet-allwinner-add-gmac200-support.patch
1140-net-ethernet-allwinner-add-gmac-support.patch
#1141-irqchip-sunxi-nmi-Support-Allwinner-A523-NMI-control.patch
1150-arm64-dtsi-allwinner-add-initial-A523-support.patch
1151-arm64-dtsi-allwinner-add-gmac1-in-A523-dtsi.patch
1152-arm64-dtsi-allwinner-add-gmac0-in-A523-dtsi.patch
1170-arm64-dts-allwinner-h728-add-x96q-pro-tvbox-plus.patch
1172-arm64-dts-allwinner-t527-add-orangepi-4a-dts.patch
1173-arm64-dts-allwinner-a527-add-Radxa-A5E-support.patch
	config
        linux.preset)
#        60-linux.hook
#        90-linux.hook)

md5sums=('a7523cfaca336076830f99b355baf773'
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
         '14d6342d9f60a37220ca5d13c2648d23'
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
         'ceed8f43b31dbe1eb4e9556e972af0a9'
         '4f0853228839336c69adcb2d9dadf2b3'
         'd2955a406c37d17802961b4706ae89df'
         '0e6ebee7a6c045dd7cf45cbafbf924bb'
         '1dcafc57cdbc3421e12ab54a54c8284c'
         'f912776f05276c66311105f57fb5d475'
         '2ab5ad8b1cc31bd85ea5d642253db36b'
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
         '4c62c914bb5810e618197837bbbfce27'
         '06af7233187c50bda4eaf4e86a5165ac'
         'cb90ddcc4fdfdacc23cdc0a6f9161037'
         '05050488cbea1692873c913c518a7e91'
         'f68f47d2728f964b399f5ee302f4aaeb'
         '58f455a5626beb3e0f0ad4bf7c58a876'
         '54e9c55d7a90f00f6a6fc6d2494db9ed'
         'abe67e12862f6aab45af666d27a689ae'
         '2322b63bd374e80189211273b5e21785'
         '0bec4e3a7f3cc36da11e647b2e92330d'
         'afb7fdc35fb492c5b32b229025faff29'
         'a7bee1cf23fb624052eeb43361c20381'
         'bb1dc5da8fa5a1cdc685a0cc2e0d883f'
         '4b820f69ab2b8c22d65498791b6a3ad8'
         '8ba482f313154a54b2eeae6dff0bf5bb'
         'a956b9e7de1d253e8ad3e6f88ba58cfa'
         '861d4b535ab64007ca8129799c9d0ee1'
         'cbfa0efa5b123208b70986ed10043167'
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
         'f6d3d5ce58f3110d6c4b17af0c5720b5'
         'e7ae0a54c830f35a9eb41f8db035fc68'
         '340440939d477e453e465a2733c4f0a9'
         '6408cd90546123bd07f4f80f2b7010e3'
         '0114a1d4e4274815c6eebfcf7b1c1948'
         'c891fba63f548409549b1a96d8604680'
         '9a2c9408381d546b16e983246484fd40'
         'da75c3163ffef13cbe070ed1d75da4e3'
         '84eeeb28c18b434dbf72ba3ed5f759b2'
         'aec9fbd8c684f614d1a3a9ca89702a72'
         'b28a68bfa642929be6a92e1db7a8b759'
         '12f1da0a3013cbbd6a4724490dbc99d1'
         '98b226ad5582fa6286a2b8bdc851b1ff'
         'fbd3050b4a357d249e758c7220a14320'
         '148de4dd254cd9b1b514cf96e7cf07f3'
         '5596eed0396b37cd7a89ded4e3d2105d'
         'c6cd0cd910f8f0e9dab7797b5de3088b'
         'b53eccd45d108c9de24a42746d908f87'
         'b5d2589f111a29ebdb55da19004f0c13'
         '2770d20a46a13c8760a96b6edf01e68a'
         '9026a13127f2f2d8db75e6c21c4f027f'
         '4b04b720d2aa0a167e30cfeea0b77faf'
         '370b405625ddfd65a038b84032f807f0'
         '68f0356aa268f890f9dfda206e32ecee'
         'e8eb4d5b6d7d0c6103477813041216ec'
         'd559a352374a2becd9fb6d30c6c7b6cf'
         '6b514cb03ef096d5d2f42a8b4332d918'
         '18705fe9e7bdcfe4b1d22dddf0b6a7dd'
         '7ff3b7e09aaefa3060fb18a6bc04d367'
         '9fe69661ecc8589982ee6e25a8e39def'
         'fb23e83c63071479b59a8e8997f9c5e0'
         'ff6624ff56cb9a1db8f8fe8408e89a81'
         '48c85cf2e1b0df6bd0f8c73525e1d999'
         '8979801afff6e1407ecb61d7a7de8652'
         'a2e0c1f541044bdf845dc85182bdd685'
         '59fa47be5f410dc12516b03a7212b0e4'
         '311615576573b9312b77c1b3cfa06905'
         '2c2e654aa7616f5bb572870db57d19f0'
         'a8e731a84f47e376c3cb9f897c6e6f9d'
         'a276c207e09b37fe925c057d052332a9'
         '711f870fb612b6c040cac0347e6e0110'
         '2d479ac232348c0b8de4e40387aa1068'
         'c60570afc7764396cb1dff690e9131f5'
         'a5439686c190e9ec469c7393f069e402'
         '9b956f7aec0ab9caeaa61916a740dcba'
         '85dac6a15f92e16bee8ca7d5b310289f'
         'e41d58ab7198267e35a13267b6271517'
         '3af0e56d3f51672e583fbda323f04a65'
         'd591681a8febc01148e508e74a92a8cb'
         '3c02684aef87c95b6b9b5518c6bfe0a5'
         'cd72a9957e6de633d2f13cdeff18c250'
         'f017947770a1437b95a8ee43ef3c3230'
         '94bbcd69e543c60031441cf271c58103'
         'f81a7ef76e83e2154f2c3eedc4c9e738'
         '20e44228749195bb373be207eb0913c0'
         'a53a9c2349cbb31e0df58ffa0cb31940'
         '66c00ba9dc275d49e59913c881180dd9'
         '8410d1a68422c011dc81c2c750c6ae66'
         '67d212212e26b85a227ce64ec03b7cdc'
         '2e1e83b688993f1b4f86ddb70ce45606'
         '5465dcfebea1b7484a8e9acedf56936d'
         '56deacc1ae8413a287354f8939f50d19'
         '3c65d6f27e049bb57749c16b630bfa25'
         '5df0d1ace04cfc94a4fbb1cf82475b95'
         '174292fdfc3a507dccd906927e105d29'
         '9adf3152ee7de57427d8cbdec30fcbe8'
         'c7820b692c16c84792c4c88802da2f16'
         '0c98702836f8f63b93ab0592e136ab0b'
         'b19a0fb88c27f47d55f03b7e4d190a8e'
         'ff5354d037a69b78a087494744adb6f5'
         'c101c652cb6c6b2adb619c2f30cb73e1'
         'c47cbf6c6d85cd1cfd06b8bc015cab7b'
         '012154852c069f8646d6a158fb6b4c36'
         '6d9d629973ac27a2f2c1528ea1a4fc74'
         'abcb7183729a8517cc7fa9bacf7bea23'
         'f817c818e78749b722f12853e167682c'
         'dd2bb620bc5f7a0845095d07a41a1f36'
         'f97bab70380815da4ac94ccb32eeac6d'
         '1570f1b168f8db30445fb28bcecc44f5'
         '6b958d8de0a713d2d34704b63b79c491'
         'b35e23b95e562ec24b29d34410c64ac0'
         'fbe9c4bde5fe180306f00004bb8a95cb'
         'e7ad4a7cd3e2932dd8c3251f5c59c6ce'
         '9611873888ea7da3bf3ba2bb7625b211'
         'cd764c04dc2b0feebac5c2c300a80a08'
         'e6d45d671cbdee3591c4012f8d2ed9f8'
         '7d653321ae7f79d08bbd58e4ac1def0b'
         '3502eb8a17aacac3df37c941461162f8'
         '8f0c414aa221b660f0bfd8c33452c04b'
         '4ac94b423b496ef513a057bbc222206d'
         '3aa15bccb1a46204c00c97c495ce7e66'
         'd060cc4b40e501349cfbd4e1a526efe2'
         'a3daeffd6291c149ee148eb7abacc356'
         '5ad2f4fae8d1e947dd98915eefe0bbe1'
         '52924aa4e7cd2b0d9ed7baaf59d620b8'
         'd3f34b921136cab564802ce8cc112d46'
         'ba20191bb8bf68e5c49feb8648e99a61'
         '8aaaaf097b997376c765234746cbe390'
         'ea98681e1f2c2737c49cf3db14a6c249'
         '4e2c1bff5da345de0ff04bf873dd0b4c'
         '9fa68366a5cc3593b432416ff6891e74'
         '2f8e3bd528618820c7553a251d0d3e10'
         'b803395f14ed05f8c7d7c3ddc682514c'
         'c9b3c7cd607bf628f3872b8f8a436da9'
         'f062d64364505698d6f27ee54069b406'
         '1b1ea7347419ec3b6a3eb360fae69c7f'
         '87159ba2177714770664fdb1262cf7a0'
         '2c90efd23f4ef77a5e373e479f9e50b1'
         '1ab580fa55e2a7f12d0ad2a9db20bb35'
         '7252e25b5a4188be520c8deb715c2f27'
         'b79c8ad7d58028348a5b37c2599b4d13'
         'c6f52ab98b5a171e75ca9ef68bceb146'
         '62d3dd3c1e5594f998fad4d9b393fd3d'
         '2dd2ab43ddaeb8727ee2ea25b40322df'
         'd162daf02d02f2b9546de8e3a517e0c4'
         '04138aa89414aeec9edb1e642b72e982'
         'a240fa074688d4510314b13a34a1c481'
         'a9eafe300ac4e670606b4e141ef69bc6'
         '60ad12926f305185b3799c1ced352114'
         '9092131879a95ab80306f0f64bf1ff9f'
         '949fba1c3087911f49841233f0ae5747'
         '2eb7348561933d031cd8ecfc8ed418a7'
         '655565572764a843a5061ff81f42bbeb'
         '2b512006b108042407cf828c5e63f788'
         '74fb0cc09ea3ff5c460f992a36687480'
         'ec0c81d851dfa6d244d71d501c681c83'
         'e138ee15bdc3f4ef0cde65784be6dad6'
         'd1ea38bc8105ae09d19442012036d60d'
         'c563e195e06db3202c75db8c915b4610'
         'f1892b3d62c80940551d09b0e46d7d66'
         '809de75a53d53969058414449162840b'
         '42844580144cf8228b07f2bc7b1b41da'
         '15922aad03494acae5bceba28c35999f'
         'c8ac7a4c7669c07cb8398b7b1c254a6b'
         '8dfbd82ba81432c44ccfce6ed917783c'
         '167aa614b573d4caea6692c3b7088a6c'
         '6be853d77b89be46412b9a0a108a2b4d'
         'e7b2222a8ab06b237986c164d6f73225'
         '7d25b8c9d5795e34195ace5a0b42e858'
         '3179ab015496807bbf1f97c9a0cd6dbb'
         '0f6f9ac070c3055eca1e69cc42f84c09'
         'cbdf37d89b99b0235cfddfb4dbf636f4'
         '9d6935352f4d5639ccfb3e602edfb30f'
         '8dd72a8fce108f4d5c3881afcab76826'
         '92b5ffe1204ccda8852357e6c8931ba5'
         '553a60026b108e1061be901f54199831'
         '34433e10ee95e684df2991127d50d7a4'
         'd4392674f9d700a5bbd7c1ddd8c07e94'
         'fc2aae58f0f5641aab21748d74ff4cf7'
         '494c74c17d54fcd623b7bdd0b4ea2299'
         '4cdc0e2a20b54bda7730ef26f1d34694'
         '6dcab0586d2dd7025502f6edbba07be6'
         'ef7951f77136006c01f878a02d418e19'
         'af732661ff052d2065406a80926db245'
         '38590334132664eecf24e9dfbd58c9f3'
         '08086fd33fa42b2e4c574211bdf4f313'
         '6986195ae8251c1eda9a7ec6ef071e47'
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
