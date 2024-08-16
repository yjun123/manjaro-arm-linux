# AArch64 multi-platform
# Maintainer: Dan Johansen <strit@manjaro.org>
# Contributor: Kevin Mihelich <kevin@archlinuxarm.org>
# Contributor: Dragan Simic <dsimic@buserror.io>

pkgbase=linux
pkgver=6.10.5
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
source=(#"https://cdn.kernel.org/pub/linux/kernel/v6.x/${_srcname}.tar.xz"
	"https://mirrors.edge.kernel.org/pub/linux/kernel/v6.x/${_srcname}.tar.xz"
"0108-drivers-led-add-openvfd-g3118dda3.patch"
#"0109-drm-panfrost-add-support-for-custom-soft-reset-on-GXM.patch" #Does not Apply on 6.10
"0110-drivers-net-wireless-brcmfmac-add-ap6330-firmware.patch"
"0125-drm-lima-dvfs-switch-gov-to-performance.patch"
"0126-drm-panfrost-dvfs-switch-gov-to-performance.patch"
"0311-arm64-dts-meson-set-dma-pool-to-896MB.patch"
"0312-g12-set-cma-to-896MiB-for-4k.patch"
"0329-media-meson-vdec-esparser-check-parsing-.patch"
"0330-media-meson-vdec-implement-10bit-bitstre.patch"
"0331-media-meson-vdec-add-HEVC-decode-codec.patch"
"0332-media-meson-vdec-disable-MPEG1-MPEG2-hardware-de.patch"
"0341-arm64-meson-add-Amlogic-Meson-GX-PM-Suspend.patch"
"0342-arm64-dts-meson-add-support-for-GX-PM-and-Virtu.patch"
"0361-arm64-dts-meson-gxm-add-beelink-gt1.patch"
"0371-arm64-dts-meson-sm1-add-support-for-TX5-plus.patch"
"0377-drm-meson-swap-primary-overlay-zpos.patch"
"0500-clk-Implement-protected-clocks-for-all-OF-clock-prov.patch"
"0501-Revert-clk-qcom-Support-protected-clocks-property.patch"
"0502-arm64-dts-allwinner-h6-Protect-SCP-clock.patch"
"0503-rtc-sun6i-Allow-RTC-wakeup-after-shutdown.patch"
"0504-firmware-arm_scpi-Support-unidirectional-mailbox-cha.patch"
"0505-arm64-dts-allwinner-h6-Add-SCPI-protocol.patch"
"0506-ASoC-hdmi-codec-fix-channel-allocation.patch"
"0507-ASoC-sun4i-i2s-WiP-multi-channel.patch"
"0508-arm64-dts-sun50i-h6-dtsi-add-sound-node.patch"
"0524-arm64-dts-allwinner-h6-Fix-Cedrus-IOMMU-again.patch"
"0531-iommu-sun50i-Allow-page-sizes-multiple-of-4096.patch"
"0534-media-cedrus-Don-t-CPU-map-source-buffers.patch"
"0535-drm-sun4i-mixer-Add-caching-support.patch"
"0536-drm-sun4i-dw-hdmi-Deinit-PHY-in-fail-path.patch"
"0537-drm-sun4i-dw-hdmi-Remove-double-encoder-cleanup.patch"
"0538-drm-sun4i-dw-hdmi-Switch-to-bridge-functions.patch"
"0539-drm-sun4i-Don-t-show-error-for-deferred-probes.patch"
"0540-drm-sun4i-dw-hdmi-Make-sun8i_hdmi_phy_get-more-intui.patch"
"0541-drm-sun4i-dw-hdmi-check-for-phy-device-first.patch"
"0542-drm-sun4i-de2-de3-Change-CSC-argument.patch"
"0543-drm-sun4i-de2-de3-Merge-CSC-functions-into-one.patch"
"0544-drm-sun4i-de2-de3-call-csc-setup-also-for-UI-layer.patch"
"0545-drm-bridge-dw-hdmi-add-mtmdsclock-parameter-to-phy-c.patch"
"0546-drm-bridge-dw-hdmi-support-configuring-phy-for-deep-.patch"
"0547-WIP-drm-sun4i-de3-Add-support-for-YUV420-output.patch"
"0549-media-Add-NV12-and-P010-AFBC-compressed-formats.patch"
"0550-media-cedrus-add-format-filtering-based-on-depth-and.patch"
"0551-media-cedrus-Implement-AFBC-YUV420-formats-for-H265.patch"
"0552-drm-sun4i-de2-Initialize-layer-fields-earlier.patch"
"0553-drm-sun4i-de3-Implement-AFBC-support.patch"
"0554-media-cedrus-Increase-H6-clock-rate.patch"
"0556-HACK-clk-sunxi-ng-unify-parent-for-HDMI-clocks.patch"
"0559-mfd-add-AC200.patch"
"0560-net-phy-Add-support-for-AC200-EPHY.patch"
"0561-arm64-dts-sun50i-h6.dtsi-add-ac200-nodes.patch"
"0562-arm64-dts-allwinner-gs1-fix-eMMC-and-incr-vcpu-limit.patch"
"0563-arm64-dts-allwinner-tanix-tx6-mini-enable-eth.patch"
"0564-arm64-dts-allwinner-add-Eeachlink-H6-Mini.patch"
"0565-arm64-dts-allwinner-tanix-tx6-mini-enable-wifi-cpu-dvfs.patch"
"0567-arm64-dts-enable-audio-gs1.patch"
"0568-arm64-dts-allwinner-tanix-tx6-enable-wifi-cpu-dvfs.patch"
"0569-drm-dw-hdmi-cec-sleep-100ms-on-error.patch"
"0570-arm64-dts-sun50i-h6-normalize-spdif-card-name.patch"
"0573-mmc-sunxi-fix-unusuable-eMMC-on-some-H6-boards-by-di.patch"
"0575-H6-add-sun50i-di-deinterlace-WiP.patch"
"0576-arm64-dts-h6-add-deinterlace-node.patch"
"0577-net-wireless-add-xr819-support-07072021.patch"
"0579-drm-bridge-dw-hdmi-fix-4k60-modes-on-some-tv.patch"
"0580-net-stmmac-sun8i-Use-devm_regulator_get-for-PHY-regu.patch"
"0581-net-stmmac-sun8i-Rename-PHY-regulator-variable-to-re.patch"
"0582-net-stmmac-sun8i-Add-support-for-enabling-a-regulato.patch"
"0583-arm64-dts-allwinner-orange-pi-3-Enable-ethernet.patch"
"0584-bluetooth-btrtl-add-hci-ver-rtl8822cs.patch"
"0585-arm64-dts-allwinner-OrangePi3-fixes.patch"
"0586-hantro-Add-quirk-for-NV12-NV12_4L4-capture-format.patch"
"0587-arm64-dts-allwinner-add-Tanix-TX6-A.patch"
"0588-arm64-dts-allwinner-enable-gpu-opp-multiple-boards.patch"
"0590-arm64-dts-allwinner-add-orangepi-3-lts.patch"
"0592-arm64-dtsi-allwinner-rework-cpu-gpu-opp.patch"
"0600-drivers-h616-wip-add-usb-emac2-support.patch"
"0601-drivers-thermal-allwinner-add-h616-ths-support.patch"
"0602-media-cedrus-add-H616-variant.patch"
"0603-soc-sunxi-sram-Add-SRAM-C1-H616-handling.patch"
"0606-dma-sun6i-dma-add-h616-support.patch"
"0607-drivers-drm-wip-add-h616-hdmi-jernejsk-24102023.patch"
"0608-sound-soc-sunxi-add-codec-driver-for-h616.patch"
"0609-sound-soc-add-sunxi_v2-for-h616-ahub.patch"
"0614-clk-sunxi-ng-ccu-sun6i-rtc-fix-32k-clk.patch"
"0615-drivers-iommu-sun50i-iommu-fix-iommu-on-h616.patch"
"0616-net-wireless-add-uwe5622-support-v20231020.patch"
"0617-sound-soc-sunxi-add-spdif-spdif.patch"
"0618-sound-soc-sunxi-hack-to-fix-oops-on-cards-caps-query.patch"
"0630-arm64-dts-allwinner-h616.dtsi-add-audio-hdmi-vdec.patch"
"0631-arm64-dts-allwinner-h616.dtsi-add-ths-cpu-gpu-opp-and-dvfs.patch"
"0632-arm64-dts-allwinner-h616.dtsi-add-emac1.patch"
"0633-arm64-dts-allwinner-h616.dtsi-fix-x96q-failing-mmc3.patch"
"0641-arm64-dts-allwinner-h616-OrangePI-Zero23-enable-ths-hdmi-audio.patch"
"0642-arm64-dts-allwinner-h616-add-Tanix-TX6s-TVbox.patch"
"0643-arm64-dts-allwinner-h616-add-Tanix-TX6s-axp313-TVbox.patch"
"0644-arm64-dts-allwinner-h313-add-x96q-TVbox.patch"
"0645-arm64-dts-allwinner-h313-add-x96q-lpddr3-TVbox.patch"
"0647-arm64-dts-allwinner-h618-add-vontar-h618-TVbox.patch"
"0648-arm64-dts-allwinner-h618-add-opi-2w.patch"
"0650-arm64-dts-allwinner-h313-Tanix-TX1-TVbox.patch"
"0651-arm64-dts-allwinner-h313-add-x96q-v5.1-TVbox.patch"
"0703-media-v4l2-common-Add-helpers-to-calculate-bytesperl.patch"
"0704-media-v4l2-Add-NV15-and-NV20-pixel-formats.patch"
"0705-media-rkvdec-h264-Use-bytesperline-and-buffer-height.patch"
"0706-media-rkvdec-h264-Don-t-hardcode-SPS-PPS-parameters.patch"
"0707-media-rkvdec-Extract-rkvdec_fill_decoded_pixfmt-into.patch"
"0708-media-rkvdec-Move-rkvdec_reset_decoded_fmt-helper.patch"
"0709-media-rkvdec-Extract-decoded-format-enumeration-into.patch"
"0710-media-rkvdec-Add-image-format-concept.patch"
"0711-media-rkvdec-Add-get_image_fmt-ops.patch"
"0712-media-rkvdec-h264-Support-High-10-and-4-2-2-profiles.patch"
"0714-media-rkvdec-Add-HEVC-backend.patch"
"0715-media-rkvdec-Add-variants-support.patch"
"0716-media-rkvdec-Implement-capability-filtering.patch"
"0717-media-rkvdec-Add-RK3288-variant.patch"
"0718-media-rkvdec-Disable-QoS-for-HEVC-and-VP9-on-RK3328.patch"
"0722-v4l2-wip-iep-driver.patch"
"0724-media-rkvdec-add-soft-reset-on-errors.patch"
"0725-drm-rockchip-vop-add-immutable-zpos-property-fix-z-order.patch"
"0727-drm-rockchip-vop2-rk356x-reorder-wins-fix-osd-in-drm-planes.patch"
"0739-arm64-dtsi-rockchip-rk3328-rk3399-add-soft-reset.patch"
"0740-arm64-dts-rockchip-var-fixes-from-libreelec.patch"
"0743-arm64-dts-rockchip-beelink-a1-enable-openvfd.patch"
"0746-arm64-dts-rockchip-beelink-a1-bump-cpu-gpu-freqs.patch"
"0747-arm64-dts-rockchip-beelink-a1-limit-sdmmc-clk-to-35MHz.patch"
"0749-phy-rockchip-phy-add-rockchip-inno-usb3.patch"
"0750-arm64-dts-rockchip-enable-inno-usb3-beelinkA1-roc-cc.patch"
"0753-arm64-dts-rockchip-rk3399-radxa-rockpi-bc-remove-wifi-compatible.patch"
"0754-arm64-dts-rockchip-rk33xx-set-userled-to-mmc.patch"
"0755-arm64-dts-rockchip-rk3399-add-orangepi-4-and-4-lts.patch"
"0756-arm64-dts-rockchip-rk33xx-add-eth-wifi-aliases.patch"
"0800-Enable-rk356x-PCIe-controller.patch"
"0801-net-wireless-backport-aic8800-sdio-v2024_0327_3561b08f.patch"
"0802-net-wireless-mm2-fixes-aic8800-sdio-v2024_0327_3561b08f.patch"
"0803-net-wireless-backport-aic8800-usb-v2024_0116_ec460377.patch"
"0804-net-wireless-mm2-fixes-aic8800-usb-v2024_0116_ec460377.patch"
"0805-media-rockchip-introduce-rkvdec2-driver.patch"
"0806-media-rockchip-rkvdec2-add-hevc-support.patch"
"0831-arm64-dts-rockchip-enable-usb2-usb3-sata-audio-in-rk35xx.dtsi.patch"
"0832-arm64-dtsi-rockchip-rk356x-disable-vepu-rga-enable-dfi.patch"
"0833-arm64-dts-rockchip-enable-Quartz64-A-usb2-usb3-pcie-audio.patch"
"0836-arm64-dts-rockchip-add-dts-for-x96-x6.patch"
"0840-arm64-dts-rockchip-add-dts-for-rock3b.patch"
"0841-arm64-dts-rockchip-increas-alarm-cpu-temp-to-85.patch"
"0842-arm64-dts-rockchip-Quartz64-B-fix-Eth-enable-hdmi-audio.patch"
"0843-arm64-dts-rockchip-rock3a-fix-mdio-reset-disable-uart-bt.patch"
"0845-arm64-dts-rockchip-add-dts-for-rock3c.patch"
"0846-arm64-dts-rockchip-rk35xx-set-userled-to-mmc.patch"
"0847-arm64-dts-rockchip-add-dts-for-urve-pi.patch"
"0848-arm64-dts-rockchip-add-dts-for-opi-3b.patch"
"0849-arm64-dts-rockchip-add-dts-for-zero3.patch"
"0850-arm64-dts-rockchip-rk356x-add-eth-wifi-aliases.patch"
"0900-rpi-vc04_services-add_h~l2-m2m_decode-15062024.patch"
#"0900-rpi-vc04_services-add_h~l2-m2m_decode-25022024.patch"
"0901-rpi-vc04_services-bcm2835-codec-remove-isp-formats.patch"
"0902-media-add-rpivid-driver.patch"
"0905-drivers-add-rpi5-clk-pinctrl-mmc-pwm-net-usb-pci-rp1.patch"
"0906-gpu-drm-vc4-add-rpi5-support.patch"
"0907-hack-dma-vc4-add-rpi5-audio-support.patch"
"0950-arm64-dts-brcm-set-userled-to-mmc.patch"
"0951-arm64-dts-brcm-add-rpi5-dt.patch"
"0952-arm64-dts-broadcom-Add-in-DRM-pipeline-to-2712.patch"
"0953-arm64-dts-add-rpivid-rpi4-rpi5.patch"
"0954-arm64-dts-disable-hdmi-audio-on-2712.patch"
#"0955-arm64-dts-add-audio-support-rpi5.patch"
"1002-irqchip-fix-its-timeout-issue.patch"
"1005-crypto-rockchip-rk3688-add-crypto-support.patch"
"1006-char-hw_random-add-rk3588s-support.patch"
"1007-media-hantro-g1-add-video-decoder-support-v1.patch"
"1011-math.h-add-DIV_ROUND_UP_NO_OVERFLOW.patch"
"1012-clk-divider-Fix-divisor-masking-on-64-bit-platforms.patch"
"1013-clk-composite-replace-open-coded-abs_diff.patch"
"1014-clk-rockchip-rk3588-drop-unused-code.patch"
"1015-clk-rockchip-handle-missing-clocks-with-EPROBE_DEFER.patch"
"1016-clk-rockchip-rk3588-register-GATE_LINK-later.patch"
"1017-clk-rockchip-expose-rockchip_clk_set_lookup.patch"
"1018-clk-rockchip-fix-error-for-unknown-clocks.patch"
"1019-clk-rockchip-implement-linked-gate-clock-support.patch"
"1020-clk-rockchip-rk3588-drop-RK3588_LINKED_CLK.patch"
"1021-phy-rockchip-samsung-hdptx-Add-FRL-EARC-supp.patch"
"1022-phy-rockchip-samsung-hdptx-Add-clock-provide.patch"
"1023-phy-rockchip-samsung-hdptx-Add-verbose-l.patch"
"1024-drm-rockchip-vop2-Improve-display-modes-handling.patch"
"1025-drm-bridge-dw-hdmi-Simplify-clock-handling.patch"
"1026-drm-bridge-dw-hdmi-Move-common-data-to-separate-head.patch"
"1027-drm-bridge-dw-hdmi-Commonize-dw_hdmi_i2c_adapter.patch"
"1028-drm-bridge-dw-hdmi-Commonize-AVI-infoframe-setup.patch"
"1029-drm-bridge-dw-hdmi-Commonize-vmode-setup.patch"
"1030-drm-bridge-dw-hdmi-Commonize-hdmi_data_info-setup.patch"
"1031-drm-bridge-dw-hdmi-Commonize-dw_hdmi_connector_creat.patch"
"1032-drm-rockchip-dw_hdmi-Use-modern-drm_device-based-log.patch"
"1033-drm-rockchip-dw_hdmi-Simplify-clock-handling.patch"
"1034-drm-rockchip-dw_hdmi-Use-devm_regulator_get_enable.patch"
"1035-drm-bridge-synopsys-Add-DW-HDMI-QP-TX-controller-dri.patch"
"1036-drm-rockchip-dw_hdmi-Add-basic-RK3588-support.patch"
"1037-drm-rockchip-dw_hdmi-rockchip-Simplify-hack-to-pass-pixel-clock-r.patch"
"1038-drm-rochchip-dw_hdmi-rockchip-HPD-cleanup.patch"
"1039-drm-vop2-add-clock-resets-support.patch"
"1040-ASoC-rockchip-add-machine-driver-for-hdmi-audio.patch"
"1041-ASoC-rockchip-hdmi-support-dts-specified-daifmt.patch"
"1042-ASoC-rockchip-hdmi-Fix-potential-NULL-point-referenc.patch"
"1043-ASoC-rockchip-i2s-tdm-Add-support-for-Digital-Loopba.patch"
"1044-ASoC-rockchip-i2s-tdm-Add-support-for-PATHx-controls.patch"
"1045-drm-bridge-synopsys-add-audio-support-in-dw-hdmi-qp.patch"
"1046-drm-bridge-synopsys-dw-hdmi-qp-workaround-for-hisense-tv.patch"
"1047-drm-bridge-synopsys-dw-hdmi-qp-add-cec-wip.patch"
"1048-net-ethernet-add-yt6801-gige-pcie-controller.patch"
"1049-net-ethernet-yt6801-gige-pcie-silence-debug-msgs.patch"
"1070-arm64-dtsi-rk3588s-add-vop2-clock-resets.patch"
"1071-arm64-dtsi-rockchip-3588s-add-cpufreq-support.patch"
"1072-arm64-dtsi-rockchip-3588s-add-crypto-support.patch"
"1073-arm64-dtsi-rockchip-3588s-add-hw_rng-support.patch"
"1074-arm64-dtsi-rockchip-3588s-add-hdmi0-bridge.patch"
"1075-arm64-dtsi-rockchip-3588s-add-rkvdec2.patch"
"1076-arm64-dtsi-rockchip-3588s-add-hdmi-audio.patch"
"1077-arm64-dtsi-rockchip-3588-add-hdmi1-bridge.patch"
"1078-arm64-dtsi-rockchip-3588s-enable-cec-on-hdmi0.patch"
"1080-arm64-dts-rockchip-rk3588-rock5x-add-cpufreq-support.patch"
"1081-arm64-dts-rockchip-rk3588-opi5x-rock5x-enable-gpu-nodes.patch"
"1082-arm64-dts-rockchip-rk3588-opi5x-rock5x-make-led-mmc0-act.patch"
"1083-arm64-dts-add-hdmi0-nodes-rock5x-orange5x.patch"
"1084-arm64-dts-add-rock5c-dt.patch"
"1085-arm64-dts-rockchip-rk3588-opi5x-add-missing-nodes.patch"
"1086-arm64-dts-rockchip-rk3588-rock5ab-add-missing-nodes.patch"
"1087-arm64-dts-rockchip-rock5x-opi5x-add-rkvdec2.patch"
"1088-arm64-dts-add-hdmi-audio-nodes-rock5x-orange5x.patch"
"1089-arm64-dts-enable-pwm-fan-rock5x-orange5x.patch"
"1090-arm64-dts-rockchip-add-rock5itx-board.patch"
"1091-arm64-dts-rockchip-add-opi5pro-board.patch"
#"1100-dt-bindings-clock-add-rk3528-clock-definitions.patch"
#"1101-clk-rockchip-add-clock-controller-for-the-RK3528.patch"
#"1102-pinctrl-rockchip-add-rk3528-support.patch"
#"1103-dt-bindings-power-add-RK3528-SoCs-header-for-idle.patch"
#"1104-ethernet-stmmac-dwmac-rk3528-add-GMAC-support.patch"
#"1105-soc-rockchip-power-domain-add-rk3528-support.patch"
#"1106-phy-rockchip-inno-usb2-add-phy-support-for-rk3528.patch"
#"1108-soc-rockchip-power-domain-add-rk3528-support.patch"
#"1108-thermal-rockchip-add-support-for-rk3528.patch"
#"1109-phy-rockchip-naneng-combphy-add-support-for-rk3528.patch"
#"1110-phy-rockchip-inno-hdmi-add-support-for-rk3528.patch"
#"1111-drm-rockchip-dw_hdmi-add-support-for-rk3528.patch"
#"1113-nvmem-rockchip-otp-add-support-for-rk3528.patch"
#"1114-sound-soc-codecs-add-rk3528-support.patch"
#"1115-hack-hack-gpu-drm-rockchip-rockchip_vop2_reg-add-rk3528.patch"
#"1150-arm64-dtsi-rockchip-add-3528.dtsi.patch"
#"1151-arm64-dts-rockchip-add-dts-for-vontar_r3.patch"
#"1152-arm64-dts-rockchip-rk3528-add-dts-for-rock2a.patch"
	'config'
        'linux.preset'
        '60-linux.hook'
        '90-linux.hook')
md5sums=('276ef1f11ed3713ec5d6f506ff55ac12'
         '3b74abbcd8ee0b9499e728830a31c108'
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
         '948d2b29d83ef6e8fcce6e929c166e05'
         'cf5203f2097037076840055e10e2b378'
         'fac6a4de3708bb8a2423a12a592120bb'
         '4668886e40c0c9bc2ea4f62868803e4a'
         'a7e8181374ada3419a3922c4e10d46da'
         '554fd010bfcfd195deeaaa5a180499b9'
         'e61dbbef63849e7523c9847f0e4618db'
         '1699b20e867741a86c35d743b4a17df4'
         'cb47353acc35d5ef90d2c4a1f51ef6e1'
         'ff3e22baa0060cbc6b8d7956b166680e'
         '5e1b41877efd5ed491c3c375acc8c654'
         '95b517e62538ac03f522e8a5b3660fb8'
         'ee87f7f93441497058fb3ebbc386a2c1'
         '852eae6e396daac53bc4a32693fd9647'
         '2d8e3a65a196bab6dec559a1d8010d21'
         '16d53d2cf9c7a265670d7f8598e298ce'
         '294c3f250b5afa17f57e79944c4d529f'
         'd28b7ed9ab5ffb4080d2ab07caac26b9'
         '2f28d6a7ee59fd6b4693346a9df93beb'
         '461b9f84cf0daea89f1bdbfba27b0279'
         'cfc48c553aab7fdf43ce1f288d7d7b33'
         '67633bce93c27a2f264a17373dd5b32a'
         '1f1d8ae4ede5f0679310b65076749a2e'
         'c3e9d498c6b413e157433d6a509a81b4'
         '046df9d0731dc40f24406fe01626680b'
         '339c96261bce31d4e70635380ec0a6b4'
         '39790f191e61387817480a50899600a9'
         'ceed8f43b31dbe1eb4e9556e972af0a9'
         'e60cf63f431af5766e13ff4c626b2ad0'
         '20020f2212f2d414cfd342fbd3c886ac'
         '4f0853228839336c69adcb2d9dadf2b3'
         '8488af1e862c67cf7e41753b96aeea6b'
         'e9d5b81c6db0a2e3724f02ca9c52d25a'
         'e9e3cd4057e870fc34d701d4542cc3ec'
         'aa19151df8770f0fa126a93fade5d115'
         '428d69fd2f4fcb96af7c5a9aad9af780'
         '1d11d026d9644bc7c9bf8a13c39f4362'
         '638b58066a16da62c6eee019e7db5803'
         'd90fe549764b44cdc542290f5d5cb080'
         '2d31c924cee504820c08c9b08b10e0af'
         '0c6f8d51d8d9f2b0d2ac9fe09acf1a66'
         '7377e24f367aefded32626d68036637f'
         'd02ce5bb9d708eefb4fb3120d27c681a'
         '0e6ebee7a6c045dd7cf45cbafbf924bb'
         'af96a8475a70397f2e65ab07088259ad'
         'e2bf8a4a8706706ef53879c6e0238db4'
         '5f73f77065196e91f2e4455388bb454f'
         'e4a4657990a54cdc00f8ecb322aa6049'
         '082667b0867720fcc338f8cf93cc7314'
         '7ed076b3fc61d2a405934d301ecf1643'
         '440cb89d09ccb6ac72bff2ae811f1950'
         '2e37e312337cb16fc57d5b782f26098b'
         '1dcafc57cdbc3421e12ab54a54c8284c'
         '5259409dc93c0806efc5a7cfaf79f3e6'
         '2ab5ad8b1cc31bd85ea5d642253db36b'
         '0b6d168d526c86fae23a0e5ad60aeaf9'
         '0f9f0572d73d09e262a8684d1cb7972a'
         '92b0ea4ef05a765139b277aad7509b50'
         '12cea7e2a3e7f6882976440e1bb504af'
         'f443813381896cb685b0012b1d7108d4'
         '42db2fae3d4fc7435de7f756d12d456c'
         '63e44cc95a8b2ede6a5f8ee830e795bc'
         '226ff38d2a1ead67c4457210b2f8f42f'
         '590861813b731c3783645007146b0d09'
         '1565568ca247a3bd83ca3c010957cf7d'
         'e3b858bf6d8c214e3d7d6b1fe7a28c1c'
         'c1eee7f21c1f41d84fab1429618f68b9'
         'f68f47d2728f964b399f5ee302f4aaeb'
         '13066a3d6122e0327d0825a833a09b31'
         'd3716111fc8d8271a344809f5836fdbe'
         '06af7233187c50bda4eaf4e86a5165ac'
         'cb90ddcc4fdfdacc23cdc0a6f9161037'
         '05acdd45b2c4b380e042ad873c70a9ff'
         '4ad4aa7964c01cb3cb8fa5f5f0334689'
         'abe67e12862f6aab45af666d27a689ae'
         '2322b63bd374e80189211273b5e21785'
         '5f6536fcd2a0fdeb998cd1dc5f44615d'
         'afb7fdc35fb492c5b32b229025faff29'
         'a7bee1cf23fb624052eeb43361c20381'
         '67d5468cd17f9def87c80083c1218e04'
         'a0698465eb7baf345ea77686406a25ce'
         '8ba482f313154a54b2eeae6dff0bf5bb'
         '14acc6fb20afc441c9625c0d498849c2'
         '4fac389e63b73c757112b84d9dd0d090'
         '07ccda7e85ea8ff3f05261b92cf83a85'
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
         '1e7bac7ab300d8ce51022c8eff5e3359'
         'f6d3d5ce58f3110d6c4b17af0c5720b5'
         'e7ae0a54c830f35a9eb41f8db035fc68'
         '340440939d477e453e465a2733c4f0a9'
         '0c383de57c0b02c7accb13bde2bca967'
         'de23727d0762f23aed00c37718a28fcf'
         'c891fba63f548409549b1a96d8604680'
         '9a2c9408381d546b16e983246484fd40'
         'da75c3163ffef13cbe070ed1d75da4e3'
         '561b88669aff22803139d8108f8c616e'
         'b28a68bfa642929be6a92e1db7a8b759'
         '12f1da0a3013cbbd6a4724490dbc99d1'
         'e59597e912ad943a84709d79460fbe83'
         '23df2aec25ffe1797809191571f00303'
         '148de4dd254cd9b1b514cf96e7cf07f3'
         'c6cd0cd910f8f0e9dab7797b5de3088b'
         'b53eccd45d108c9de24a42746d908f87'
         'ed6f6037a1b01b2669ea346815cc6318'
         '2770d20a46a13c8760a96b6edf01e68a'
         '4482cdd8cf4564b9a3b37662091406e8'
         '6d4f0de9e038326a1d9725da44156a24'
         '1a0a8576101f0a07684d71af28242c55'
         '4b04b720d2aa0a167e30cfeea0b77faf'
         '370b405625ddfd65a038b84032f807f0'
         '68f0356aa268f890f9dfda206e32ecee'
         'd559a352374a2becd9fb6d30c6c7b6cf'
         '0806874e4c92de067a0a962ec3156408'
         '18705fe9e7bdcfe4b1d22dddf0b6a7dd'
         '7ff3b7e09aaefa3060fb18a6bc04d367'
         '9fe69661ecc8589982ee6e25a8e39def'
         'b1f17ef2afe6c9f34c1e3edebce74dbc'
         '52f41871a46dd799ea3c4d0388a56aa4'
         '0a6604ad9b5e3414459ff5fba884b736'
         '9e97409c4c2e2499fda5578b56885bdb'
         'd0c86f089a373685cfeab4a8b8044d1d'
         '2181d88aff47486fe30314f7c24d96bd'
         'c1de13c843db4dd06fef4673d222c2e0'
         '2c2e654aa7616f5bb572870db57d19f0'
         '0d2384945be6c776bd57a2e7efaded57'
         '476a1ab292ee93cbd05eea377723e7d4'
         '8069f599ec23e166d47e90df8081d4db'
         '6e6316f8cb8acead972eb765245cd442'
         '3bd11e927c995fbfad6308de4fc2d300'
         'aa3f2502665899ac354c80bc5f0ffc83'
         '6e97c36c1bfb4305ac38672d50036c5e'
         '671e0b345f6c2d0b69ec2b173d388223'
         'cc4fff1612f3765fcc4b276bc3a7b93e'
         '99bd886f8297e15779df841c4f8ce186'
         'ac620d2fc3b559b577d26d77487f1f3d'
         'c1fc160cc201186b2c6924c8a23d1775'
         '59ce9e0d4f71e80f6a963d34666e3101'
         '601fcba79dd0fe4059e2cc7f0ea5ba9f'
         '55578cf90077c7feb56d8a74619891c9'
         '53692153d99c0d538e4737b44f2091dc'
         '5e3729e0f4660c2f3964166d3f93fcf1'
         'c2113afed10822a0c3668b0b52367585'
         'f6cbe2a8e0a44c427b72b6eab5cfc149'
         '5d1a2f72a79f899fb6e681765bb18c7f'
         '09f654d234acbff9b96c7b6bb4c947c8'
         '453c38179c860ab3e00e26e8a8371620'
         '612721fa3b76c4f8dad18ff847e2cbe4'
         '313e88b11d64381b189a538bac625d73'
         '0627c6aa0c083ba4428681ecaf02cb16'
         '4dbef3f09fee65726207be395c9fffaa'
         '9fb8ce76577b20cfea07affa05b8160d'
         'd32a321fd43b34bf5d7e4fde715a3300'
         '1faafe6030e6c675697383d90fe7b0c5'
         'a924c67baa56578111a08573f540e8a0'
         '71bba35e9fcd6a790a57c20a7f3afa1f'
         '77970876770f83500c49bf71c74e478e'
         '1b60afd3448033cbca923492fb756441'
         '58ba740b6b413565f6342b1eff761cff'
         'b1ae2a11b7e25ceb1acd5c5ef835188c'
         'ee17dd75ccd8c2180aa79c0285700e17'
         'ee0bd3b4b55f16be786b61c2ea0d438f'
         'd7f6b9b2fae86206e383c7c91fe02f97'
         'd68bacf098f5917e48228fc08955e035'
         '43cc0688eb90b63c9ceeed5eca145a09'
         'cd97f265ad6ecba7f4bb59213acda833'
         'a57e6a87a4cb0dfd5069c7113e0f2946'
         'fd732cc5df71ef6380f1f51cef8d4c0b'
         '6cf0ac596dc45a2a3e9068ce45d3950e'
         '4419de58536046d6caf48d350d2a1e74'
         'bebd26b2f07a6abc7f6931a437493b16'
         'b6868aaeadd252a1f6f68ece2d3644e8'
         '2653da71182b918be505b5254386ea89'
         'a5505789e38b08cd3962131f198c6e55'
         '9491b25efcc74ac96f6ca5af9b67ee30'
         '7d653321ae7f79d08bbd58e4ac1def0b'
         '3502eb8a17aacac3df37c941461162f8'
         '196abd0617146fd8f5e2160d9f2bc13b'
         '2c5003235ce3e7013a83bed6903db5c9'
         '0aad002daeaf2f0715c1631ffbc9c8dc'
         '1eb3cd6d8a8ccf46743e59c00f0ed0f9'
         '4406a1b051268a7e820073d8e26b19f0'
         '542220d1d2577894138eab8049fc96c4'
         '4e958b9fb9e33eb9810ee45e66164e28'
         'b7c1626df9f32824b20b4aff60151c3a'
         '5439070c9b5e322b8d44e9f139e3c3bb'
         'a49fb0c0449225b58a47e1776d223ab7'
         '0b8ff696f0151dafd8cd0614a497d4f5'
         'f5f1f62ab9d15c679c5e09c11b367c5e'
         '1ac0f1567dd2f09a6e8d723f32a71603'
         '17c66868be18faca59e3f726033b46a1'
         '0acbcb086bfe81c1e6d48d0ce080a10b'
         '2c872fcd267f38244d6f8121d7a6aea2'
         'ab9b7969b588a61f37794b6897e6812f'
         'a3d8b3483337a3f03bf37b667feaaa37'
         'e70029654e8504ee3df382b16fcc2f9a'
         'cde4b68d24b85cd20c35fa7330080b5d'
         'f1d74be5d638b98fc33cd940c01dc263'
         'dd912b8120f3e4e42d83c9844ae28e1b'
         '86d4a35722b5410e3b29fc92dae15d4b'
         'ce6c81ad1ad1f8b333fd6077d47abdaf'
         '3dc88030a8f2f5a5f97266d99b149f77')


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

  # Assorted Pinebook, PinePhone and PineTab patches
  apply_patches 1
  
  # Assorted rk356x patches
  apply_patches 2

  # Pinebook Pro patches by Megi: https://github.com/torvalds/linux/compare/master...megous:linux:pbp-6.2
  # apply_patches 4

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
  replaces=('linux-armv8' 'linux-aarch64')
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
  sed "${_subst}" ../60-linux.hook |
    install -Dm644 /dev/stdin "${pkgdir}/usr/share/libalpm/hooks/60-${pkgbase}.hook"
  sed "${_subst}" ../90-linux.hook |
    install -Dm644 /dev/stdin "${pkgdir}/usr/share/libalpm/hooks/90-${pkgbase}.hook"
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
