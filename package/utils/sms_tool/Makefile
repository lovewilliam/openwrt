include $(TOPDIR)/rules.mk

PKG_NAME:=sms_tool
PKG_VERSION:=1.0.0
PKG_RELEASE:=1

PKG_BUILD_DIR:=$(BUILD_DIR)/sms_tool-$(PKG_VERSION)
PKG_SOURCE:=sms_tool-$(PKG_VERSION).tar.gz
PKG_SOURCE_URL:=@SF/sms_tool
PKG_MD5SUM:=64fd496a7aa0c48bbf72ee78c5f3ce32
PKG_CAT:=zcat

include $(INCLUDE_DIR)/package.mk

define Package/sms_tool
  SECTION:=base
  CATEGORY:=Network
  DEFAULT:=y
  TITLE:=sms tool
  URL:=http://github.com/lovewilliam
endef

define Package/PKG_NAME/description
	3g modem sms tool (read, send sms from modem)
endef

define Package/sms_tool/install
        $(INSTALL_DIR) $(1)/usr/sbin
	$(INSTALL_BIN) $(PKG_BUILD_DIR)/sms_tool $(1)/usr/sbin/
endef

$(eval $(call BuildPackage,sms_tool))

