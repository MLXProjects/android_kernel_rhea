# bcmdhd
DHDCFLAGS = -Wall -Wstrict-prototypes -Dlinux -DBCMDRIVER                     \
        -DBCMDONGLEHOST -DUNRELEASEDCHIP -DBCMDMA32 -DWLBTAMP -DBCMFILEIMAGE  \
        -DDHDTHREAD -DDHD_GPL -DDHD_SCHED -DDHD_DEBUG -DBDC                   \
        -DDHD_BCMEVENTS -DSHOW_EVENTS -DDONGLEOVERLAYS -DBCMDBG               \
        -DCUSTOMER_HW_SAMSUNG -DOOB_INTR_ONLY                                 \
        -DMMC_SDIO_ABORT -DBCMSDIO -DBCMLXSDMMC -DBCMPLATFORM_BUS -DWLP2P     \
        -DNEW_COMPAT_WIRELESS -DWIFI_ACT_FRAME -DARP_OFFLOAD_SUPPORT          \
        -DKEEP_ALIVE -DCSCAN -DPKT_FILTER_SUPPORT                             \
        -DEMBEDDED_PLATFORM 
#-DPNO_SUPPORT

# distinguish between the 43xx chip
ifeq ($(CONFIG_BCM4334),m)
DHDCFLAGS += -DBCM4334_CHIP -DHW_OOB -DBCM4334_CHECK_CHIP_REV
DHDCFLAGS += -DUSE_CID_CHECK -DCONFIG_CONTROL_PM
DHDCFLAGS += -DPROP_TXSTATUS
DHDCFLAGS += -DVSDB -DHT40_GO
DHDCFLAGS += -DWL_CFG80211_VSDB_PRIORITIZE_SCAN_REQUEST
DHDCFLAGS += -DDHD_USE_IDLECOUNT
DHDCFLAGS += -DSUPPORT_AMPDU_MPDU_CMD
DHDCFLAGS += -DVSDB_DYNAMIC_F2_BLKSIZE -DVSDB_F2_BLKSIZE=64
#-DSDIO_F2_BLKSIZE=512 
DHDCFLAGS += -DROAM_ENABLE -DROAM_API -DROAM_CHANNEL_CACHE
endif
ifeq ($(CONFIG_BCM4334),y)
DHDCFLAGS += -DBCM4334_CHIP -DHW_OOB -DBCM4334_CHECK_CHIP_REV
DHDCFLAGS += -DUSE_CID_CHECK -DCONFIG_CONTROL_PM
DHDCFLAGS += -DPROP_TXSTATUS
DHDCFLAGS += -DVSDB -DHT40_GO
DHDCFLAGS += -DWL_CFG80211_VSDB_PRIORITIZE_SCAN_REQUEST
DHDCFLAGS += -DDHD_USE_IDLECOUNT
DHDCFLAGS += -DSUPPORT_AMPDU_MPDU_CMD
DHDCFLAGS += -DVSDB_DYNAMIC_F2_BLKSIZE -DVSDB_F2_BLKSIZE=64 
#-DSDIO_F2_BLKSIZE=512
DHDCFLAGS += -DROAM_ENABLE -DROAM_API -DROAM_CHANNEL_CACHE
endif
ifeq ($(CONFIG_BCM4330),m)
DHDCFLAGS += -DBCM4330_CHIP
DHDCFLAGS += -DMCAST_LIST_ACCUMULATION
DHDCFLAGS += -DCONFIG_CONTROL_PM
endif

ifeq ($(CONFIG_BCM4330),y)
DHDCFLAGS += -DBCM4330_CHIP
DHDCFLAGS += -DMCAST_LIST_ACCUMULATION
DHDCFLAGS += -DCONFIG_CONTROL_PM
endif
ifeq ($(CONFIG_BCM43241),m)
DHDCFLAGS += -DBCM43241_CHIP -DHW_OOB
DHDCFLAGS += -DMCAST_LIST_ACCUMULATION
DHDCFLAGS += -fno-pic
endif
ifeq ($(CONFIG_BCM43241),y)
DHDCFLAGS += -DBCM43241_CHIP -DHW_OOB
DHDCFLAGS += -DMCAST_LIST_ACCUMULATION
endif

ifeq ($(CONFIG_MACH_RHEA_SS_AMAZING),y)
DHDCFLAGS += -UHW_OOB -UUSE_CID_CHECK
DHDCFLAGS += -UHT40_GO -UPNO_SUPPORT
DHDCFLAGS += -DRDWR_MACADDR -DBCMHOST_XTAL_PU_TIME_MOD
DHDCFLAGS += -DSDIO_F2_BLKSIZE=64
endif
ifeq ($(CONFIG_MACH_RHEA_SS_LUCAS),y)
DHDCFLAGS += -UHW_OOB -UUSE_CID_CHECK
DHDCFLAGS += -UHT40_GO -UPNO_SUPPORT
DHDCFLAGS += -DRDWR_MACADDR -DBCMHOST -DBCMHOST_XTAL_PU_TIME_MOD
DHDCFLAGS += -DSDIO_F2_BLKSIZE=64
endif
ifeq ($(CONFIG_MACH_RHEA_SS_ZANIN),y)
DHDCFLAGS += -UHW_OOB -UUSE_CID_CHECK
DHDCFLAGS += -UHT40_GO -UPNO_SUPPORT
DHDCFLAGS += -DRDWR_MACADDR -DBCMHOST -DBCMHOST_XTAL_PU_TIME_MOD
DHDCFLAGS += -DSDIO_F2_BLKSIZE=64
endif
ifeq ($(CONFIG_MACH_RHEA_SS_IVORY),y)
DHDCFLAGS += -UHW_OOB -UUSE_CID_CHECK
DHDCFLAGS += -UHT40_GO -UPNO_SUPPORT
DHDCFLAGS += -DRDWR_MACADDR -DBCMHOST -DBCMHOST_XTAL_PU_TIME_MOD
DHDCFLAGS += -DSDIO_F2_BLKSIZE=64
endif
ifeq ($(CONFIG_MACH_RHEA_SS_IVORYSS),y)
DHDCFLAGS += -UHW_OOB -UUSE_CID_CHECK
DHDCFLAGS += -UHT40_GO -UPNO_SUPPORT
DHDCFLAGS += -DRDWR_MACADDR -DBCMHOST -DBCMHOST_XTAL_PU_TIME_MOD
DHDCFLAGS += -DSDIO_F2_BLKSIZE=64
endif
ifeq ($(CONFIG_MACH_RHEA_SS_CORSICA),y)
DHDCFLAGS += -UHW_OOB -UUSE_CID_CHECK
DHDCFLAGS += -UHT40_GO -UPNO_SUPPORT
DHDCFLAGS += -DRDWR_MACADDR -DBCMHOST -DBCMHOST_XTAL_PU_TIME_MOD
DHDCFLAGS += -DSDIO_F2_BLKSIZE=64
endif
ifeq ($(CONFIG_MACH_RHEA_SS_NEVIS),y)
DHDCFLAGS += -UHW_OOB -UUSE_CID_CHECK
DHDCFLAGS += -UHT40_GO -UPNO_SUPPORT
DHDCFLAGS += -DRDWR_MACADDR -DBCMHOST -DBCMHOST_XTAL_PU_TIME_MOD
DHDCFLAGS += -DSDIO_F2_BLKSIZE=64
endif
ifeq ($(CONFIG_MACH_RHEA_SS_NEVISP),y)
DHDCFLAGS += -UHW_OOB -UUSE_CID_CHECK
DHDCFLAGS += -UHT40_GO -UPNO_SUPPORT
DHDCFLAGS += -DRDWR_MACADDR -DBCMHOST -DBCMHOST_XTAL_PU_TIME_MOD
DHDCFLAGS += -DSDIO_F2_BLKSIZE=64
endif
ifeq ($(CONFIG_MACH_RHEA_SS),y)
DHDCFLAGS += -UHW_OOB -UUSE_CID_CHECK
DHDCFLAGS += -UHT40_GO -UPNO_SUPPORT
DHDCFLAGS += -DRDWR_MACADDR -DBCMHOST -DBCMHOST_XTAL_PU_TIME_MOD
DHDCFLAGS += -DSDIO_F2_BLKSIZE=64
endif

# For p2p connection issue
DHDCFLAGS += -DWL_CFG80211_GON_COLLISION
DHDCFLAGS += -DWL_CFG80211_SYNC_GON_TIME
#end p2p connection

# For Passing all multicast packets to host when not in suspend mode.
DHDCFLAGS += -DPASS_ALL_MCAST_PKTS

#For INITIAL 2G scan features

ifneq ($(CONFIG_TARGET_LOCALE_KOR),y)
DHDCFLAGS += -DUSE_INITIAL_2G_SCAN_ORG
endif


# For Scan result patch
DHDCFLAGS += -DESCAN_RESULT_PATCH

ifeq ($(CONFIG_MACH_SAMSUNG_ESPRESSO),y)
DHDCFLAGS += -DREAD_MACADDR -DHW_OOB
endif

ifeq ($(CONFIG_MACH_SAMSUNG_ESPRESSO_10),y)
DHDCFLAGS += -DREAD_MACADDR -DHW_OOB
endif

ifeq ($(CONFIG_MACH_U1),y)
DHDCFLAGS += -DUSE_CID_CHECK -DU1_MACADDR
ifeq ($(CONFIG_TARGET_LOCALE_KOR),y)
DHDCFLAGS += -DRDWR_MACADDR
else
DHDCFLAGS += -DWRITE_MACADDR
endif
endif

ifeq ($(CONFIG_MACH_SAMSUNG_T1),y)
DHDCFLAGS += -DUSE_CID_CHECK -DWRITE_MACADDR
endif

ifeq ($(CONFIG_TARGET_LOCALE_KOR),y)
DHDCFLAGS += -DOKC_SUPPORT
ifeq ($(CONFIG_BCM4334),y)
DHDCFLAGS += -DRDWR_KORICS_MACADDR
else
DHDCFLAGS += -DRDWR_MACADDR
endif
#DHDCFLAGS += -DOKC_DEBUG
#DHDCFLAGS += -DSOFTAP_DISABLE_WMM
endif

ifeq ($(CONFIG_MACH_U1_KOR_KT), y)
DHDCFLAGS += -DVLAN_MODE_OFF
DHDCFLAGS += -DKEEP_ALIVE_PACKET_PERIOD_30_SEC
DHDCFLAGS += -DFULL_ROAMING_SCAN_PERIOD_60_SEC
endif

# For Static Buffer
ifeq ($(CONFIG_BROADCOM_WIFI_RESERVED_MEM),y)
DHDCFLAGS += -DCONFIG_DHD_USE_STATIC_BUF
endif

# For CCX
ifeq ($(CONFIG_BRCM_CCX),y)
DHDCFLAGS += -DBCMCCX
endif

# For Korean domestic projects
# DHDCFLAGS += -DROAM_CHANNEL_CACHE
# DHDCFLAGS += -DROAM_ENABLE
# DHDCFLAGS += -DROAM_API
# DHDCFLAGS += -DOKC_SUPPORT

ifneq ($(findstring GlobalConfig, $(wildcard $(srctree)/include/sec_feature/*)),)
DHDCFLAGS += -DUSE_SECFEATURE
endif

ifeq ($(CONFIG_TARGET_LOCALE_CHN),y)
DHDCFLAGS += -DBCMWAPI_WPI -DBCMWAPI_WAI
endif

#For WAPI Porting on Zanin
ifeq ($(TARGET_PRODUCT),zaninzc)
DHDCFLAGS += -DBCMWAPI_WPI -DBCMWAPI_WAI
endif


# For SLP feature
ifeq ($(CONFIG_SLP),y)
DHDCFLAGS += -DSLP_PATH -DCUSTOMER_HW_SLP
endif
# GGSM_WIFI_5GHz_CHANNELS feature is define for only GGSM model
ifeq ($(GGSM_WIFI_5GHz_CHANNELS),true)
DHDCFLAGS += -DCUSTOMER_SET_COUNTRY
endif

# NAT keepalive packet filter for GAN-lite
ifeq ($(SEC_MODEL_NAME),U1)
         ifeq ($(X_BUILD_LOCALE),EUR_ORG)
              DHDCFLAGS += -DGAN_LITE_NAT_KEEPALIVE_FILTER
         endif
endif

# For Debug
EXTRA_CFLAGS += $(DHDCFLAGS) -DWL_CFG80211 -DRSSI_OFFSET=0
EXTRA_CFLAGS += -DDHD_DEBUG -DSRCBASE=\"$(src)/src\"

EXTRA_CFLAGS += -I$(src)/src/include/
EXTRA_CFLAGS += -I$(src)/src/dhd/sys/
EXTRA_CFLAGS += -I$(src)/src/dongle/
EXTRA_CFLAGS += -I$(src)/src/bcmsdio/sys/
EXTRA_CFLAGS += -I$(src)/src/wl/sys/
EXTRA_CFLAGS += -I$(src)/src/shared/
EXTRA_CFLAGS += -I$(src)/src/wl/bcmwifi/src/
EXTRA_CFLAGS += -I$(src)/src/wl/bcmwifi/include/

EXTRA_LDFLAGS += --strip-debug
KBUILD_CFLAGS += -I$(LINUXDIR)/include -I$(shell pwd)

obj-m   += dhd.o

dhd-y := src/bcmsdio/sys/bcmsdh.o	src/bcmsdio/sys/bcmsdh_linux.o \
	 src/bcmsdio/sys/bcmsdh_sdmmc.o	src/bcmsdio/sys/bcmsdh_sdmmc_linux.o \
	 src/dhd/sys/dhd_bta.o		src/dhd/sys/dhd_cdc.o \
	 src/dhd/sys/dhd_common.o	src/dhd/sys/dhd_custom_gpio.o \
	 src/dhd/sys/dhd_custom_sec.o \
	 src/dhd/sys/dhd_linux.o	src/dhd/sys/dhd_linux_sched.o \
	 src/dhd/sys/dhd_cfg80211.o	src/dhd/sys/dhd_sdio.o \
	 src/shared/aiutils.o		src/shared/bcmevent.o \
	 src/shared/bcmutils.o		src/wl/bcmwifi/src/bcmwifi_channels.o \
	 src/shared/hndpmu.o		src/shared/linux_osl.o \
	 src/shared/sbutils.o		src/shared/siutils.o \
	 src/wl/sys/wl_android.o	src/wl/sys/wl_cfg80211.o \
	 src/wl/sys/wl_cfgp2p.o		src/wl/sys/wldev_common.o \
	 src/wl/sys/wl_linux_mon.o	src/wl/sys/wl_roam.o

all:
	@echo "$(MAKE) --no-print-directory -C $(KDIR) SUBDIRS=$(CURDIR) modules"
	@$(MAKE) --no-print-directory -C $(KDIR) \
		SUBDIRS=$(CURDIR) modules

clean:
	rm -rf *.o *.ko *.mod.c *~ .*.cmd \
	Module.symvers modules.order .tmp_versions modules.builtin \
	src/bcmsdio/sys/*.o \
	src/bcmsdio/sys/*.o.cmd \
	src/bcmsdio/sys/.*.o.cmd \
	src/dhd/sys/*.o \
	src/dhd/sys/*.o.cmd \
	src/dhd/sys/.*.o.cmd \
	src/shared/*.o \
	src/shared/*.o.cmd \
	src/shared/.*.o.cmd \
	src/wl/sys/*.o \
	src/wl/sys/*.o.cmd \
	src/wl/sys/.*.o.cmd \
	src/wl/bcmwifi/src/bcmwifi_channels.o \
	src/wl/bcmwifi/src/.*.o.cmd

install:
	@$(MAKE) --no-print-directory -C $(KDIR) \
		SUBDIRS=$(CURDIR) modules_install
