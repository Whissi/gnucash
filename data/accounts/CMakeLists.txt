SET(accounts_SUBDIRS
  C
  ca
  cs
  da
  de_AT
  de_CH
  de_DE
  el_GR
  en_GB
  es_ES
  es_MX
  fi_FI
  fr_CA
  fr_CH
  fr_FR
  hu_HU
  it
#  ja
  ko
  lt
  lv
#  nb
#  nl
  pl
  pt_BR
  pt_PT
  ru
  sk
  sv_AX
  sv_FI
  sv_SE
  tr_TR
  zh_CN
  zh_HK
  zh_TW
)

SET(ACCOUNTS_INSTALL_DIR ${CMAKE_INSTALL_DATADIR}/gnucash/accounts)
SET(ACCOUNTS_BUILD_DIR ${DATADIR_BUILD}/gnucash/accounts)



ADD_SUBDIRECTORY(C)
ADD_SUBDIRECTORY(ca)
ADD_SUBDIRECTORY(cs)
ADD_SUBDIRECTORY(da)
ADD_SUBDIRECTORY(de_AT)
ADD_SUBDIRECTORY(de_CH)
ADD_SUBDIRECTORY(de_DE)
ADD_SUBDIRECTORY(el_GR)
ADD_SUBDIRECTORY(en_GB)
ADD_SUBDIRECTORY(es_ES)
ADD_SUBDIRECTORY(es_MX)
ADD_SUBDIRECTORY(fi_FI)
ADD_SUBDIRECTORY(fr_CA)
ADD_SUBDIRECTORY(fr_CH)
ADD_SUBDIRECTORY(fr_FR)
ADD_SUBDIRECTORY(hu_HU)
ADD_SUBDIRECTORY(it)
ADD_SUBDIRECTORY(ja)
ADD_SUBDIRECTORY(ko)
ADD_SUBDIRECTORY(lt)
ADD_SUBDIRECTORY(lv)
ADD_SUBDIRECTORY(nb)
ADD_SUBDIRECTORY(nl)
ADD_SUBDIRECTORY(pl)
ADD_SUBDIRECTORY(pt_BR)
ADD_SUBDIRECTORY(pt_PT)
ADD_SUBDIRECTORY(ru)
ADD_SUBDIRECTORY(sk)
ADD_SUBDIRECTORY(sv_AX)
ADD_SUBDIRECTORY(sv_FI)
ADD_SUBDIRECTORY(sv_SE)
ADD_SUBDIRECTORY(tr_TR)
ADD_SUBDIRECTORY(zh_CN)
ADD_SUBDIRECTORY(zh_HK)
ADD_SUBDIRECTORY(zh_TW)

SET_LOCAL_DIST(dist_list CMakeLists.txt )

SET(accounts_DIST ${C_DIST} ${CA_DIST} ${CS_DIST} ${DA_DIST} ${DE_AT_DIST} ${DE_CH_DIST} ${DE_DE_DIST} ${EL_GR_DIST}
                  ${EN_GB_DIST} ${ES_ES_DIST} ${ES_MX_DIST} ${FI_FI_DIST} ${FR_CA_DIST} ${FR_CH_DIST}
                  ${FR_FR_DIST} ${HU_HU_DIST} ${IT_DIST} ${JA_DIST} ${KO_DIST} ${LT_DIST} ${LV_DIST}
                  ${NB_DIST} ${NL_DIST} ${PL_DIST} ${PT_BR_DIST} ${PT_PT_DIST} ${RU_DIST} ${SK_DIST}
                  ${SV_AX_DIST} ${SV_FI_DIST} ${SV_SE_DIST} ${TR_TR_DIST} ${ZH_CN_DIST}
                  ${ZH_HK_DIST} ${ZH_TW_DIST} ${dist_list} PARENT_SCOPE)

