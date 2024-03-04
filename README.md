
## İÇİNDEKİLER
 
#KISALTMALAR 
#TANIMLAR 

* [1KISALTMALAR 5](#1 KISALTMALAR 5)
* [TANIMLAR 7](#TANIMLAR 7)
  * [1.1 Format of the Audit Log Event](#11-format-of-the-audit-log-event)
    * [1.1.1 Extended Audit Log Format](#111-extended-audit-log-format)
    * [1.1.2 Common Value Structures of the Data Fields](#112-common-value-structures-of-the-data-fields)
  * [1.2 References](#12-references)
* [2 Audit Log Events](#2-audit-log-events)
  * [2.1 Central Server](#21-central-server)
    * [2.1.1 Common Events](#211-common-events)
    * [2.1.2 Initialization Event](#212-initialization-event)
    * [2.1.3 Members Events](#213-members-events)
    * [2.1.4 Security Servers Events](#214-security-servers-events)
    * [2.1.5 Global Groups Events](#215-global-groups-events)
    * [2.1.6 Certification Services Events](#216-certification-services-events)
    * [2.1.7 Timestamping Services Events](#217-timestamping-services-events)
    * [2.1.8 Management Requests Events](#218-management-requests-events)
    * [2.1.9 Configuration Management Events](#219-configuration-management-events)
    * [2.1.10 System Settings Events](#2110-system-settings-events)
    * [2.1.11 Backup and Restore Events](#2111-backup-and-restore-events)
  * [2.2 Security Server](#22-security-server)
    * [2.2.1 Common Events](#221-common-events)
    * [2.2.2 Initialization Events](#222-initialization-events)
    * [2.2.3 Security Server Clients Events](#223-security-server-clients-events)
    * [2.2.4 System Parameters Events](#224-system-parameters-events)
    * [2.2.5 Keys and Certificates Events](#225-keys-and-certificates-events)
    * [2.2.6 Backup and Restore Events](#226-backup-and-restore-events)
    * [2.2.7 API Key Management Events](#227-api-key-management-events)
    * [2.2.8 Technical Events](#228-technical-events)
  * [2.3 Utility signer-console](#23-utility-signer-console)






 
 [KISALTMALAR	5](#KISALTMALAR	5)
TANIMLAR	7
GİRİŞ	11
Amaç ve Kapsam	11
Rehberin İçeriği ve Güncelleme Süreci	12
Rehber Uyum Planı	13
BİLGİ VE İLETİŞİM GÜVENLİĞİ REHBERİ UYGULAMA SÜRECİ	19
Planlama	21
2.1.1.	Varlık Gruplarının Belirlenmesi	21
2.1.2.	Varlık Grubu Kritiklik Derecesinin Belirlenmesi	24
2.1.3.	Mevcut Durum ve Boşluk Analizi	27
2.1.4.	Rehber Uygulama Yol Haritasının Hazırlanması	29
Uygulama	30
2.2.1. Bilgi ve İletişim Güvenliği Temel Prensipleri	30
Kontrol Etme ve Önlem Alma	31
2.3.1.	Rehber Uygulama Yol Haritasının İzlenmesi ve Kontrol Edilmesi	31
2.3.2.	Bilgi ve İletişim Güvenliği Denetimi	31
Değişiklik Yönetimi	32
2.4.1.	Rehber Değişikliklerinin Yönetilmesi	32
2.4.2.	Varlık Gruplarının Değişikliklerinin Yönetilmesi	32
VARLIK GRUPLARINA YÖNELİK GÜVENLİK TEDBİRLERİ	35
Ağ ve Sistem Güvenliği	35
3.1.1.	Donanım Varlıklarının Envanter Yönetimi	36
3.1.2.	Yazılım Varlıklarının Envanter Yönetimi	38
3.1.3.	Tehdit ve Zafiyet Yönetimi	40
3.1.4.	E-Posta Sunucusu ve İstemcisi Güvenliği	44
3.1.5.	Zararlı Yazılımlardan Korunma	47
3.1.6.	Ağ Güvenliği	49
3.1.7.	Veri Sızıntısı Önleme	57
3.1.8.	İz ve Denetim Kayıtlarının Tutulması ve İzlenmesi	59
3.1.9.	Sanallaştırma Güvenliği	61
3.1.10.	Siber Güvenlik Olay Yönetimi	64
3.1.11.	Sızma Testleri ve Güvenlik Denetimleri	66
3.1.12.	Kimlik Doğrulama ve Erişim Yönetimi	68
3.1.13.	Felaket Kurtarma ve İş Sürekliliği Yönetimi	74
3.1.14.	Uzaktan Çalışma	79
Uygulama ve Veri Güvenliği	84
3.2.1.	Kimlik Doğrulama	84
1
 
3.2.2.	Oturum Yönetimi	89
3.2.3.	Yetkilendirme	91
3.2.4.	Dosyaların ve Kaynakların Güvenliği	92
3.2.5.	Güvenli Kurulum ve Yapılandırma	95
3.2.6.	Güvenli Yazılım Geliştirme	98
3.2.7.	Veri Tabanı ve Kayıt Yönetimi	100
3.2.8.	Hata Ele Alma ve Kayıt Yönetimi	104
3.2.9.	İletişim Güvenliği	106
3.2.10.	Kötücül İşlemleri Engelleme	107
3.2.11.	Dış Sistem Entegrasyonlarının Güvenliği	111
Taşınabilir Cihaz ve Ortam Güvenliği	114
3.3.1.	Akıllı Telefon ve Tablet Güvenliği	114
3.3.2.	Taşınabilir Bilgisayar Güvenliği	118
3.3.3.	Taşınabilir Ortam Güvenliği (CD/DVD, Taşınabilir Bellek Ortamları)	120
Nesnelerin İnterneti (IoT) Cihazlarının Güvenliği	121
3.4.1.	Ağ Servisleri ve İletişimi	121
3.4.2.	Dâhili Veri Depolama	123
3.4.3.	Kimlik Doğrulama ve Yetkilendirme	124
3.4.4.	API ve Bağlantı Güvenliği	125
3.4.5.	Diğer Güvenlik Tedbirleri	126
Personel Güvenliği	128
3.5.1.	Genel Güvenlik Tedbirleri	128
3.5.2.	Eğitim ve Farkındalık Faaliyetleri	131
3.5.3.	Tedarikçi İlişkileri Güvenliği	132
Fiziksel Mekânların Güvenliği	134
3.6.1.	Genel Güvenlik Tedbirleri	135
3.6.2.	Sistem Odası/Veri Merkezine Yönelik Güvenlik Tedbirleri	141
3.6.3.	Elektromanyetik Bilgi Kaçaklarından Korunma Yöntemleri (TEMPEST)	146
UYGULAMA VE TEKNOLOJİ ALANLARINA YÖNELİK GÜVENLİK TEDBİRLERİ	149
Kişisel Verilerin Güvenliği	149
4.1.1.	Kayıt Yönetimi	149
4.1.2.	Erişim Kayıtları Yönetimi	152
4.1.3.	Yetkilendirme	153
4.1.4.	Şifreleme	155
4.1.5.	Yedekleme, Silme, Yok Etme ve Anonim Hale Getirme	156
4.1.6.	Aydınlatma Yönetimi	157
4.1.7.	Açık Rıza Yönetimi	158
4.1.8.	Kişisel Veri Yönetim Sürecinin İşletilmesi	160
Anlık Mesajlaşma Güvenliği	161
4.2.1. Genel Güvenlik Tedbirleri	161
Bulut Bilişim Güvenliği	163
4.3.1. Genel Güvenlik Tedbirleri	164
Kripto Uygulamaları Güvenliği	168
4.4.1.	Kriptografik Algoritmalar ve Kullanımı	168
4.4.2.	Şifreleme ve Anahtar Yönetimi	170
4.4.3.	Kriptografik Uygulamalar	176
Kritik Altyapılar Güvenliği	178
4.5.1.	Genel Güvenlik Tedbirleri	178
4.5.2.	Enerji Sektörü Özelinde Güvenlik Tedbirleri	179
4.5.3.	Elektronik Haberleşme Sektörü Özelinde Güvenlik Tedbirleri	182
Yeni Geliştirmeler ve Tedarik	185
4.6.1. Genel Güvenlik Tedbirleri	185
SIKILAŞTIRMA TEDBİRLERİ	189
İşletim Sistemi Sıkılaştırma Tedbirleri	189
5.1.1.	Genel Sıkılaştırma Tedbirleri	189
5.1.2.	Linux İşletim Sistemi Sıkılaştırma Tedbirleri	193
5.1.3.	Windows İşletim Sistemi Sıkılaştırma Tedbirleri	196
Veri Tabanı Sıkılaştırma Tedbirleri	198
5.2.1. Genel Sıkılaştırma Tedbirleri	198
Sunucu Sıkılaştırma Tedbirleri	202
5.3.1.	Web Sunucusu Sıkılaştırma Tedbirleri	203
5.3.2.	Sanallaştırma Sunucusu Sıkılaştırma Tedbirleri	207
KAYNAKÇA	210
EKLER	211
EK-A: GENELGE MADDELERİ EŞLEŞTİRME TABLOSU	211
EK-B: ULUSLARARASI STANDARTLAR VE YAYIMLI KILAVUZLAR EŞLEŞTİRME TABLOSU	215
EK-C: BİLGİ VE İLETİŞİM GÜVENLİĞİ REHBERİ UYGULAMA SÜRECİ KAPSAMINDA
KULLANILACAK FORMLAR, ŞABLONLAR VE ÖRNEK DOKÜMANLAR	217
EK-C.1: VARLIK GRUBU KRİTİKLİK DERECELENDİRME ANKETİ	217
EK-C.2: VARLIK GRUBU VE KRİTİKLİK DERECESİ TANIMLAMA FORMU	223
EK-C.3: MEVCUT DURUM VE BOŞLUK ANALİZ FORMU	224
EK-C.4: REHBER UYGULAMA YOL HARİTASI BELİRLEME FORMU	226
EK-C.5: TELAFİ EDİCİ KONTROL KAYIT FORMU	227
EK-C.6: TAAHHÜTNAME ÖRNEĞİ	228
 

ŞEKİLLER
Şekil 1. Bilgi ve İletişim Güvenliği Rehberinin Hedefleri	12
Şekil 2. Rehber Güncelleme Süreci	13
Şekil 3. Rehber Uyum Planı	13
Şekil 4. Rehber ve Bilgi Güvenliği Yönetim Sistemi İlişkisi	14
Şekil 5. Bilgi ve İletişim Güvenliği Rehberi Uygulama Süreci	19
Şekil 6. Varlıklar, Varlık Grupları ve Varlık Ana Başlıkları	22
Şekil 7. Kritiklik Derecesi Belirlemek için Kullanılan Boyutlar	24
Şekil 8. Temel Prensipler	30


TABLOLAR
Tablo 1. SAM Rolleri Açıklamaları	20
Tablo 2. Bilgi ve İletişim Güvenliği Rehberi Uygulama Süreci için Sorumluluk Atama Matrisi	20
Tablo 3. Anket Puanına Karşılık Gelen Kritiklik Derecesi	25
Tablo 4. Varlık Grubu Kritiklik Derecesinin Belirlenmesi	26
Tablo 5. Alt Varlık Gruplarının Kritiklik Derecesinin Belirlenmesi	26
Tablo 6. Varlık Gruplarına Yönelik Tedbir Uygulanabilirlik Örnek Çalışması	27









---
name: Change request
about: Suggest a change for this project
title: ''
labels: 'enhancement'
assignees: ''

---

**Describe what change you would like**
<!-- Describe below what change is needed -->

**Context**
Language: (eg 'cn' or 'pt')
Section: (eg '05-checklis')
<!-- Add below any other context or screenshots about the change request -->



# Audit log events

Version: 1.12

Doc. ID: SPEC-AL

## Version history

| Date       | Version | Description                                                                                                                                               | Author             |
|------------|---------|-----------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------|
| 11.09.2015 | 0.1     | Initial version                                                                                                                                           | Kristo Heero       |
| 14.09.2015 | 0.2	    | Bug fixes                                                                                                                                                 | Kristo Heero       |
| 16.09.2015 | 0.3     | 	Made editorial changes in introduction                                                                                                                   | Margus Freudenthal |
| 18.09.2015 | 1.0     | Editorial changes made                                                                                                                                    | Imbi Nõgisto       |
| 09.10.2015 | 1.1     | Delete certificate/key events of security server updated                                                                                                  | Kristo Heero       |
| 12.10.2015 | 1.2     | Updated CSR generation events. Fields nameExtractorMemberClass and nameExractorMethod replaced with field certificateProfileInfo                          | Kristo Heero       |
| 20.10.2015 | 1.3     | New events 'Add subsystem' and 'Register management service provider as security server client' added                                                     | Kristo Heero       |
| 21.10.2015 | 1.4     | New fields managementRequestId and keyLabel added                                                                                                         | Kristo Heero       |
| 23.10.2015 | 1.5     | Data field of the event 'Edit WSDL' changed                                                                                                               | Kristo Heero       |
| 08.12.2015 | 1.6     | Added audit log events for TLS internal key certificate requests and certificate import                                                                   | Ilkka Seppälä      |
| 10.05.2016 | 1.7     | Merged changes from xtee6-doc repo.<br>Added New event ‘Skip unregistration of authentication certificate' added change made by Meril Vaht on 10.12.2015. | Kedi Välba         |
| 10.05.2020 | 1.8     | Updated to match current implementation                                                                                                                   | Janne Mattila      |
| 16.02.2023 | 1.9     | Converted document from docx to markdown                                                                                                                  | Raido Kaju         |
| 17.04.2023 | 1.10    | Remove central services support                                                                                                                           | Justas Samuolis    |
| 05.06.2023 | 1.11    | New Central Server                                                                                                                                        | Eneli Reimets      |
| 09.12.2023 | 1.12    | Management service TLS certificate                                                                                                                        | Eneli Reimets      |

## Table of Contents

* [1 Introduction](#1-introduction)
  * [1.1 Format of the Audit Log Event](#11-format-of-the-audit-log-event)
    * [1.1.1 Extended Audit Log Format](#111-extended-audit-log-format)
    * [1.1.2 Common Value Structures of the Data Fields](#112-common-value-structures-of-the-data-fields)
  * [1.2 References](#12-references)
* [2 Audit Log Events](#2-audit-log-events)
  * [2.1 Central Server](#21-central-server)
    * [2.1.1 Common Events](#211-common-events)
    * [2.1.2 Initialization Event](#212-initialization-event)
    * [2.1.3 Members Events](#213-members-events)
    * [2.1.4 Security Servers Events](#214-security-servers-events)
    * [2.1.5 Global Groups Events](#215-global-groups-events)
    * [2.1.6 Certification Services Events](#216-certification-services-events)
    * [2.1.7 Timestamping Services Events](#217-timestamping-services-events)
    * [2.1.8 Management Requests Events](#218-management-requests-events)
    * [2.1.9 Configuration Management Events](#219-configuration-management-events)
    * [2.1.10 System Settings Events](#2110-system-settings-events)
    * [2.1.11 Backup and Restore Events](#2111-backup-and-restore-events)
  * [2.2 Security Server](#22-security-server)
    * [2.2.1 Common Events](#221-common-events)
    * [2.2.2 Initialization Events](#222-initialization-events)
    * [2.2.3 Security Server Clients Events](#223-security-server-clients-events)
    * [2.2.4 System Parameters Events](#224-system-parameters-events)
    * [2.2.5 Keys and Certificates Events](#225-keys-and-certificates-events)
    * [2.2.6 Backup and Restore Events](#226-backup-and-restore-events)
    * [2.2.7 API Key Management Events](#227-api-key-management-events)
    * [2.2.8 Technical Events](#228-technical-events)
  * [2.3 Utility signer-console](#23-utility-signer-console)

## License

This work is licensed under the Creative Commons Attribution-ShareAlike 3.0 Unported License. To view a copy of this
license, visit http://creativecommons.org/licenses/by-sa/3.0/.

## 1 Introduction

X-Road central and security servers keep audit log. The audit log events are generated by user interfaces when the user
changes system state or configuration. Additionally, the utility `signer-console` generates audit log events. The user
actions are logged regardless of whether the outcome was a success or a failure.

This document provides complete list of all audit log events and theirs related data sets.

### 1.1 Format of the Audit Log Event

The audit log record contains description of the audit log event in `JSON` format. The field event represents the
description of the event, the field user represents the user name of the performer (events started by the system have
the user name `system`), and the field data represents data fields related with the event:

```json
{
  "event": "...",
  "user": "...",
  "reason": "...",
  "data": {
    "data_field_1": "data_field_1_value", 
    ...
  }
}
```

In case of failure the event description ends with suffix failed and related data set may contain less data fields than
normally. Also, an additional field reason for the error message will be added.

Security Server and Central Server audit log contains some additional elements, described in the next chapter.

Section 2 lists all the possible (successful) event descriptions and corresponding set of data fields (some fields are
optional).

#### 1.1.1 Extended Audit Log Format

Security Server and Central Server use REST APIs to update data, and a new audit log implementation adds some features that are useful in
auditing updates done through the API.

Example of extended audit log message for the security server:
```bash
2023-05-25T13:26:32+03:00 dev-ss1.i.x-road.rocks correlation-id: [a81deb2bf312a60f] INFO  [X-Road Proxy Admin REST API] 
2023-05-25T13:26:32.409+03:00 - {
  "event":"Refresh service description",
  "user":"xrd",
  "ipaddress":"192.0.2.1",
  "auth":"Session",
  "url":"/api/v1/service-descriptions/7/refresh",
  "data":{
    "clientIdentifier":{
      "memberClass":"ORG",
      "memberCode":"111",
      "subsystemCode":"MANAGEMENT",
      "fieldsForStringFormat":["ORG","111","MANAGEMENT"],
      "objectType":"SUBSYSTEM",
      "xroadInstance":"DEV"},
   "url":"http://dev-cs.i.x-road.rocks/managementservices.wsdl",
   "serviceType":"WSDL",
   "wsdl":{
     "servicesAdded":[],
     "servicesDeleted":[]
    }
  }
}
```

Log contains (outside the actual audit log event `JSON`) `correlation-id` element which can be used to associate
audit log entry with a specific request, regular log entries and e.g. stack traces from regular log.

Audit log event `JSON` contains these additional elements:

* ipaddress
  * the IP address of the user
* auth
  * authentication type used for this API call
    * possible values:
      * Session - session based authentication (web application)
      * ApiKey - direct API call using API key authentication
      * HttpBasicPam - HTTP basic authentication with PAM login (for api key management API operations)
* url
  * url of called API endpoint
* warning
  * for failed events, boolean indicating whether the failure was caused by unhandled warnings

```json
{
  "event": "...",
  "user": "...",
  "ipaddress":"...",
  "reason": "...",
  "warning": true,
  "auth": "Session",
  "url": "/api/service-descriptions/249",
  "data": {
    "data_field_1": "data_field_1_value", 
    ...
  }
```

#### 1.1.2 Common Value Structures of the Data Fields

Values of data fields `memberIdentifier`, `clientIdentifier`, `ownerIdentifier`, `providerIdentifier`, and 
`serviceProviderIdentifier` have a common structure:

```json
{
  "xRoadInstance": "...",
  "memberClass": "...",
  "memberCode": "..."
}
```

where `xRoadInstance` is the X-Road instance, `memberClass` is the X-Road member class, and `memberCode` is the X-Road
member code. In case of `clientIdentifier`, `providerIdentifier`, and `serviceProviderIdentifier` an optional field
`subsystemCode` (the X-Road subsystem code) is present in the structure.

## 2 Audit Log Events

### 2.1 Central Server

#### 2.1.1 Common Events

The audit log events related to the UI logging and the UI language settings.

| Event           | Data fields                                |
|-----------------|--------------------------------------------|
| Log in user     |                                            |
| Log out user    |                                            |
| Set UI language | * locale - the selected UI locale (e.g en) |

#### 2.1.2 Initialization Event

The audit log event related to initialization.

| Event                     | Data fields                                                                                                                                                                                                                        |
|---------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Initialize Central Server | <ul><li>centralServerAddress - the address of the Central Server</li><li>instanceIdentifier - the instance identifier of the Central Server</li><li>haNode - the name of the node in the cluster in the case of HA setup</li></ul> |

#### 2.1.3 Members Events

The audit log events related to configuration of the X-Road members.

| Event                                        | Data fields                                                                                                                                                                                                                                                                                                                                                                                           |
|----------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Add member                                   | <ul><li>memberName - the member name of the added member</li><li>memberClass - the member class of the added member</li><li>memberCode - the member code of the added member</li></ul>                                                                                                                                                                                                                |
| Edit member name                             | <ul><li>memberName - the new member name of the edited member</li><li>memberClass - the member class of the edited member</li><li>memberCode - the member code of the edited member</li></ul>                                                                                                                                                                                                         |
| Delete member                                | <ul><li>memberClass - the member class of the deleted member</li><li>memberCode - the member code of the deleted member</li></ul>                                                                                                                                                                                                                                                                     |
| Add subsystem                                | <ul><li>memberClass - the member class of the added subsystem</li><li>memberCode - the member code of the added subsystem</li><li>memberSubsystemCode - the subsystem code of the added subsystem</li></ul>                                                                                                                                                                                           |
| Delete subsystem                             | <ul><li>memberClass - the member class of the deleted subsystem</li><li>memberCode - the member code of the deleted subsystem</li><li>memberSubsystemCode - the subsystem code of the deleted subsystem</li></ul>                                                                                                                                                                                     |
| Unregister member as security server client  | <ul><li>serverCode - the server code of the selected security server</li><li>ownerClass - the owner class of the selected security server</li><li>ownerCode - the owner code of the selected security server</li><li>clientIdentifier - the client identifier of the member unregistered as client of the selected security server</li></ul>                                                          |

#### 2.1.4 Security Servers Events

The audit log events related to configuration of the X-Road security servers.

| Event                                                | Data fields                                                                                                                                                                                                                                                                                                                                                                                                               |
|------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Edit security server address                         | <ul><li>serverCode - the server code of the edited security server</li><li>ownerCode - the owner code of the edited security server</li><li>ownerClass - the owner class of the edited security server</li><li>address - the new address of the edited security server</li></ul>                                                                                                                                          |
| Delete security server                               | <ul><li>serverCode - the server code of the deleted security server</li><li>ownerCode - the owner code of the deleted security server</li><li>ownerClass - the owner class of the deleted security server</li></ul>                                                                                                                                                                                                       |
| Delete authentication certificate of security server | <ul><li>serverCode - the server code of the selected security server</li><li>ownerCode - the owner code of the selected security server</li><li>ownerClass - the owner class of the selected security server</li><li>certHash - the hash of the deleted authentication certificate of the selected security server</li><li>certHashAlgorithm - the hash algorithm used to calculate value of the field certHash</li></ul> |

#### 2.1.5 Global Groups Events

The audit log events related to configuration of the X-Road global groups.

| Event                        | Data fields                                                                                                                                                                                                                                                  |
|----------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Add global group                 | <ul><li>code - the group code of the added global group</li><li>description - the description of the added global group</li></ul>                                                                                                                        |
| Edit global group description    | <ul><li>code - the group code of the edited global group</li><li>description - the new description of the edited global group</li></ul>                                                                                                                  | 
| Delete global group              | <ul><li>code - the group code of the deleted global group</li><li>description - the description of the deleted global group</li></ul>                                                                                                                    |
| Add members to global group      | <ul><li>code - the group code of the selected global group</li><li>description - the description of the selected global group</li><li>memberIdentifiers - the list of member identifiers of the members added to the selected global group</li></ul>     |
| Remove members from global group | <ul><li>code - the group code of the selected global group</li><li>description - the description of the selected global group</li><li>memberIdentifiers - the list of member identifiers of the members removed from the selected global group</li></ul> |

#### 2.1.6 Certification Services Events

The audit log events related to configuration of the X-Road certification services.

| Event                                       | Data fields                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
|---------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Add certification service                   | <ul><li>caId - the identifier of the added certification service</li><li>caCertHash - the hash of the CA certificate of the added certification service</li><li>caCertHashAlgorithm - the hash algorithm used to calculate value of the field caCertHash</li><li>authenticationOnly - the authentication only flag of the added certification service</li><li>certificateProfileInfo - the fully qualified (Java) class name that implements the CertificateProfileInfo interface of the added certification service</li></ul>            |
| Edit certification service settings         | <ul><li>caId - the identifier of the edited certification service</li><li>caCertHash - the hash of the CA certificate of the edited certification service</li><li>caCertHashAlgorithm - the hash algorithm used to calculate value of the field caCertHash</li><li>authenticationOnly - the (new) authentication only flag of the edited certification service</li><li>certificateProfileInfo - the fully qualified (Java) class name that implements the CertificateProfileInfo interface of the eddited certification service</li></ul> |
| Delete certification service                | <ul><li>caId - the identifier of the deleted certification service</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| Add intermediate CA                         | <ul><li>caId - the identifier of the selected certification service</li><li>intermediateCaId - the identifier of the intermediate CA added to the selected certification service</li><li>intermediateCaCertHash - the hash of the intermediate CA certificate</li><li>intermediateCaCertHashAlgorithm - the hash algorithm used to calculate value of the field intermediateCaCertHash</li></ul>                                                                                                                                          |
| Delete intermediate CA                      | <ul><li>intermediateCaId - the identifier of the deleted intermediate CA</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| Add OCSP responder of certification service | <ul><li>caId - the identifier of the selected certification service</li><li>ocspId - the identifier of the OCSP responder added to the selected certification service</li><li>ocspUrl - the URL of the added OCSP responder</li><li>ocspCertHash - the hash of the added OCSP responder certificate</li><li>ocspCertHashAlgorithm - the hash algorithm used to calculate value of the field ocspCertHash</li></ul>                                                                                                                        |
| Add OCSP responder of intermediate CA       | <ul><li>intermediateCaId - the identifier of the selected intermediate CA</li><li>ocspId - the identifier of the OCSP responder added to the selected intermediate CA</li><li>ocspUrl - the URL of the added OCSP responder</li><li>ocspCertHash - the hash of the added OCSP responder certificate</li><li>ocspCertHashAlgorithm - the hash algorithm used to calculate value of the field ocspCertHash</li></ul>                                                                                                                        |
| Edit OCSP responder                         | <ul><li>ocspId - the identifier of the edited OCSP responder</li><li>ocspUrl - the (new) URL of the edited OCSP responder</li><li>ocspCertHash - the (new) hash of the edited OCSP responder certificate</li><li>ocspCertHashAlgorithm - the hash algorithm used to calculate value of the field ocspCertHash</li></ul>                                                                                                                                                                                                                   |
| Delete OCSP responder                       | <ul><li>ocspId - the identifier of the deleted OCSP responder</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |

#### 2.1.7 Timestamping Services Events

The audit log events related to configuration of the X-Road timpestamping services.

| Event                       | Data fields                                                                                                                                                                                                                                                                                                                                                                                        |
|-----------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Add timestamping service    | <ul><li>tsaId - the identifier of the added timestamping service</li><li>tsaName - the name of the added timestamping service</li><li>tsaUrl - the URL of the added timestamping service</li><li>tsaCertHash - the hash of the timestamping service certificate</li><li>tsaCertHashAlgorithm - the hash algorithm used to calculate value of the field tsaCertHash</li></ul>                       |
| Edit timestamping service   | <ul><li>tsaId - the identifier of the edited timestamping service</li><li>tsaName - the (new) name of the edited timestamping service</li><li>tsaUrl - the (new) URL of the edited timestamping service</li><li>tsaCertHash - the hash of the edited timestamping service certificate</li><li>tsaCertHashAlgorithm - the hash algorithm used to calculate value of the field tsaCertHash</li></ul> |
| Delete timestamping service | <ul><li>tsaId - the identifier of the deleted timestamping service</li><li>tsaName - the name of the deleted timestamping service</li><li>tsaUrl - the URL of the deleted timestamping service</li></ul>                                                                                                                                                                                           |

#### 2.1.8 Management Requests Events

The audit log events related to the management requests.

| Event                      | Data fields                                                          |
|----------------------------|----------------------------------------------------------------------|
| Add management request     | <ul><li>requestId - the identifier of the added request</li></ul>    |
| Revoke management request  | <ul><li>requestId - the identifier of the revoked request</li></ul>  |
| Approve management request | <ul><li>requestId - the identifier of the approved request</li></ul> | 
| Decline management request | <ul><li>requestId - the identifier of the declined request</li></ul> |

#### 2.1.9 Configuration Management Events

The audit log events related to configuration management.

| Event                                       | Data fields                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|---------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Re-create internal configuration anchor     | <ul><li>anchorFileHash - the hash of the re-created internal configuration anchor file</li><li>anchorFileHashAlgorithm - the hash algorithm used to calculate value of the field anchorFileHash</li></ul>                                                                                                                                                                                                                                                                                                                           |
| Generate internal configuration signing key | <ul><li>tokenId - the identifier of the token used to generate the signing key</li><li>tokenSerialNumber - the serial number of the token</li><li>tokenFriendlyName - the friendly name of the token</li><li>keyId - the identifier of the generated signing key</li><li>keyFriendlyName - the friendly name of the generated key</li><li>certHash - the hash of the generated signing certificate</li><li>certHashAlgorithm - the hash algorithm used to calculate value of the field certHash</li></ul>                           |
| Activate internal configuration signing key | <ul><li>tokenId - the identifier of the token owning the signing key</li><li>tokenSerialNumber - the serial number of the token</li><li>tokenFriendlyName - the friendly name of the token</li><li>keyId - the identifier of the activated signing key</li></ul>                                                                                                                                                                                                                                                                    |
| Delete internal configuration signing key   | <ul><li>tokenId - the identifier of the token owning the signing key</li><li>tokenSerialNumber - the serial number of the token</li><li>tokenFriendlyName - the friendly name of the token</li><li>keyId - the identifier of the deleted signing key</li></ul>                                                                                                                                                                                                                                                                      |
| Re-create external configuration anchor     | <ul><li>anchorFileHash - the hash of the re-created external configuration anchor file</li><li>anchorFileHashAlgorithm - the hash algorithm used to calculate value of the field anchorFileHash</li></ul>                                                                                                                                                                                                                                                                                                                           |
| Generate external configuration signing key | <ul><li>tokenId - the identifier of the token used to generate the signing key</li><li>tokenSerialNumber - the serial number of the token</li><li>tokenFriendlyName - the friendly name of the token</li><li>keyId - the identifier of the generated signing key</li><li>keyFriendlyName - the friendly name of the generated key</li><li>certHash - the hash of the generated signing key certificate</li><li>certHashAlgorithm - the hash algorithm used to calculate value of the field certHash</li></ul>                       |
| Activate external configuration signing key | <ul><li>tokenId - the identifier of the token owning the signing key</li><li>tokenSerialNumber - the serial number of the token</li><li>tokenFriendlyName - the friendly name of the token</li><li>keyId - the identifier of the activated signing key</li></ul>                                                                                                                                                                                                                                                                    |
| Delete external configuration signing key   | <ul><li>tokenId - the identifier of the token owning the signing key</li><li>tokenSerialNumber - the serial number of the token</li><li>tokenFriendlyName - the friendly name of the token</li><li>keyId - the identifier of the deleted signing key</li></ul>                                                                                                                                                                                                                                                                      |
| Add trusted anchor                          | <ul><li>anchorFileHash - the hash of the added anchor file</li><li>anchorFileHashAlgorithm - the hash algorithm used to calculate value of the field anchorFileHash</li><li>instanceIdentifier - the X-Road instance identifier of the added anchor</li><li>generatedAt - the UTC time when anchor file was generated</li><li>anchorUrls - the configuration download URLs of the added anchor</li></ul>                                                                                                                            |
| Delete trusted anchor                       | <ul><li>anchorFileHash - the hash of the deleted anchor file</li><li>anchorFileHashAlgorithm - the hash algorithm used to calculate value of the field anchorFileHash</li><li>instanceIdentifier - the X-Road instance identifier of the deleted anchor</li></ul>                                                                                                                                                                                                                                                                   |
| Log in to token                             | <ul><li>tokenId - the identifier of the token logged in</li><li>tokenSerialNumber - the serial number of token</li><li>tokenFriendlyName - the friendly name of token</li></ul>                                                                                                                                                                                                                                                                                                                                                     |
| Log out from token                          | <ul><li>tokenId - the identifier of the token logged out</li><li>tokenSerialNumber - the serial number of token</li><li>tokenFriendlyName - the friendly name of token</li></ul>                                                                                                                                                                                                                                                                                                                                                    |
| Upload configuration part                   | <ul><li>sourceType - the source type (internal or external) of the uploaded configuration part</li><li>contentIdentifier - the content identifier of the uploaded configuration part</li><li>partFileName - the internal name of the configuration part file</li><li>uploadFileName - the name of the uploaded configuration part file</li><li>uploadFileHash - the hash of the uploaded configuration part file</li><li>uploadFileHashAlgorithm - the hash algorithm used to calculate value of the field uploadFileHash</li></ul> |

#### 2.1.10 System Settings Events

The audit log events related to the system settings.

| Event                                                          | Data fields                                                                                                                                                                                                                                                                                                                                               |
|----------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Edit Central Server address                                    | <ul><li>centralServerAddress - the new address of the Central Server</li></ul>                                                                                                                                                                                                                                                                            |
| Register management service provider as Security Server client | <ul><li>serverCode - the server code of the management services' security server</li><li>ownerClass - the owner class of the management services' security server</li><li>ownerCode - the owner code of the management services' security server</li><li>clientIdentifier - the client identifier of the registered management service provider</li></ul> |
| Edit provider of management services                           | <ul><li>serviceProviderIdentifier - the new service provider identifier of the management service</li><li>serviceProviderName - the new service provider name of the management service</li></ul>                                                                                                                                                         |
| Add member class                                               | <ul><li>code - the code of the added member class</li><li>description - the description of the added member class</li></ul>                                                                                                                                                                                                                               |
| Edit member class description                                  | <ul><li>code - the code of the edited member class</li><li>description - the new description of the edited member class</li></ul>                                                                                                                                                                                                                         |
| Delete member class                                            | <ul><li>code - the code of the deleted member class</li></ul>                                                                                                                                                                                                                                                                                             |
| API key create                                                 | <ul><li>apiKeyId - identifier of the API key</li><li>apiKeyRoles - array containing the roles associated with the API key</li></ul>                                                                                                                                                                                                                       |
| API key update                                                 | <ul><li>apiKeyId - identifier of the API key</li><li>apiKeyRoles - array containing the roles associated with the API key</li></ul>                                                                                                                                                                                                                       |
| API key remove                                                 | <ul><li>apiKeyId - identifier of the API key</li><li>apiKeyRoles - array containing the roles associated with the API key</li></ul>                                                                                                                                                                                                                       |
| Generate management service TLS key and self-sign certificate  | <ul><li>certHash - the hash of the management service TLS certificate</li><li>certHashAlgorithm - the hash algorithm used to calculate value of the field certHash</li></ul>                                                                                                                                                                              |
| Generate management service TLS certificate signing request    | <ul><li>subjectName - the subject name of the generated certificate request</li></ul>                                                                                                                                                                                                                                                                     |
| Upload management service TLS certificate                      | <ul><li>certFileName - the file name of the uploaded certificate</li><li>certHash - the hash of the uploaded certificate</li><li>certHashAlgorithm - the hash algorithm used to calculate value of the field certHash</li></ul>                                                                                                                           |
#### 2.1.11 Backup and Restore Events

The audit log events related to back up and restore.

| Event                 | Data fields                                                                                  |
|-----------------------|----------------------------------------------------------------------------------------------|
| Back up configuration | <ul><li>backupFileName - the name of the created backup file</li></ul>                       |
| Upload backup file    | <ul><li>backupFileName - the name of the uploaded backup file</li></ul>                      |
| Delete backup file    | <ul><li>backupFileName - the name of the deleted backup file</li></ul>                       |
| Restore configuration | <ul><li>backupFileName - the name of the backup file used to restore configuration</li></ul> |

### 2.2 Security Server

#### 2.2.1 Common Events

The audit log events related to the UI logging.

| Event        | Data fields |
|--------------|-------------|
| Log in user  |             |
| Log out user |             |

#### 2.2.2 Initialization Events

The audit log events related to initialization.

| Event                           | Data fields                                                                                                                                                                                                                                               |
|---------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Initialize anchor               | <ul><li>anchorFileHash - the hash of the initialized anchor file</li><li>anchorFileHashAlgorithm - the hash algorithm used to calculate value of the field anchorFileHash</li><li>generatedAt - the UTC time when the anchor file was generated</li></ul> |
| Initialize server configuration | <ul><li>ownerIdentifier - the owner identifier of the initialized security server</li><li>serverCode - the server code of the initialized security server</li></ul>                                                                                       |

#### 2.2.3 Security Server Clients Events

The audit log events related to the security server clients configuration.

| Event                                                    | Data fields                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
|----------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Add client                                               | <ul><li>clientIdentifier - the client identifier of the added client</li><li>isAuthentication - the information system authentication type of the added client</li><li>clientStatus - the status of the added client</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| Register client                                          | <ul><li>clientIdentifier - the client identifier of the registered client</li><li>managementRequestId - the identifier of the corresponding management request in the Central Server</li><li>clientStatus - the status of the registered client</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| Unregister client                                        | <ul><li>clientIdentifier - the client identifier of the unregistered client</li><li>managementRequestId - the identifier of the corresponding management request in the Central Server</li><li>clientStatus - the status of the unregistered client</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| Delete client                                            | <ul><li>clientIdentifier - the client identifier of the deleted client</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| Delete orphaned client keys, certs and certificates      | <ul><li>tokenId - the identifier of the token where the deleted key located</li><li>tokenSerialNumber - the serial number of the token</li><li>tokenFriendlyName - the friendly name of the token</li><li>keyId - the identifier of the deleted key</li><li>keyFriendlyName - the friendly name of the deleted key</li><li>keyUsage - the key usage of the deleted key</li><li>clientIdentifier - the client identifier of the client which certificates and certificate requests were deleted</li><li>certHashes - the list of hashes of the deleted certificates</li><li>certHashAlgorithm - the hash algorithm used to calculate hash values of the field certHashes</li><li>certRequestIds - the list of identifiers of the deleted certificate requests</li></ul> |
| Change owner                                             | <ul><li>clientIdentifier - the client identifier of the selected client</li><li>managementRequestId - the identifier of the corresponding management request in the Central Server</li><li>clientStatus - the status of the registered client</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| Add service description                                  | <ul><li>clientIdentifier - the client identifier of the selected client</li><li>url - the URL of the added service description of the selected client</li><li>serviceType - type of the service description: WSDL, REST, or OPENAPI3</li><li>disabled - the flag indicating whether the added WSDL and all its services were disabled</li><li>refreshedDate - the time when the added WSDL was refreshed</li></ul>                                                                                                                                                                                                                                                                                                                                                     |
| Delete service description                               | <ul><li>clientIdentifier - the client identifier of the selected client</li><li>url - the URL of the service description of the selected client</li><li>serviceType - type of the service description: WSDL, REST, or OPENAPI3</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| Disable service description                              | <ul><li>clientIdentifier - the client identifier of the selected client</li><li>url - the URL of the service description of the selected client</li><li>serviceType - type of the service description: WSDL, REST, or OPENAPI3</li><li>disabledNotice - the notice of the disabled WSDLs</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| Enable service description                               | <ul><li>clientIdentifier - the client identifier of the selected client</li><li>url - the URL of the service description of the selected client</li><li>serviceType - type of the service description: WSDL, REST, or OPENAPI3</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| Refresh service description                              | <ul><li>clientIdentifier - the client identifier of the selected client</li><li>url - the previous URL of the service description</li><li>serviceType - type of the service description: WSDL, REST, or OPENAPI3</li><li>urlNew - the new URL of the service description</li><li>wsdl - wsdl data (only for type WSDL)</li><li>servicesAdded - the list of services added during refresh</li><li>servicesDeleted - the list of services removed during refresh</li></ul>                                                                                                                                                                                                                                                                                               |
| Edit service description                                 | <ul><li>clientIdentifier - the client identifier of the selected client</li><li>url - the URL of the added service description of the selected client</li><li>serviceType - type of the service description: WSDL, REST, or OPENAPI3</li><li>wsdl - wsdl data (only for type WSDL):<li><ul><li>servicesAdded - the list of services added by the new WSDL</li><li>servicesDeleted - the list of services removed by the new WSDL</li></ul></ul>                                                                                                                                                                                                                                                                                                                        |
| Edit service parameters                                  | <ul><li>clientIdentifier - the client identifier of the member provided the edited services</li><li>url - the URL of the added service description of the selected client</li><li>serviceType - type of the service description: WSDL, REST, or OPENAPI3</li><li>services - the list of the edited services. The list item contains of the following data fields:</li><ul><li>id - the identifier of the service</li><li>url - the URL of the service</li><li>timeout - the timeout of the service</li><li>tlsAuth - the flag indicating whether the certificate of the service provider should be verified for TLS connections</li></ul></ul>                                                                                                                         |
| Add access rights to service                             | <ul><li>clientIdentifier - the client identifier of the member provided the selected service</li><li>serviceCode - the selected service code</li><li>subjectIds - the list of the selected subject identifiers to which the access of the selected service granted</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| Remove access rights from service                        | <ul><li>clientIdentifier - the client identifier of the member provided the selected service</li><li>serviceCode - the selected service code</li><li>subjectIds - the list of the selected subject identifiers from which the access of the selected service denied</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| Add access rights to subject                             | <ul><li>clientIdentifier - the client identifier of the member provided the selected service</li><li>subjectId - the selected subject identifier</li><li>serviceCodes - the list of the service codes which access granted to the selected subject</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| Remove access rights from subject                        | <ul><li>clientIdentifier - the client identifier of the member provided the selected service</li><li>subjectId - the selected subject identifier</li><li>serviceCodes - the list of the service codes which access denied to the selected subject</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| Set connection type for servers in service consumer role | <ul><li>clientIdentfier - the client identifier of the selected client</li><li>isAuthentication - the new information system authentication type of the selected client</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| Add internal TLS certificate                             | <ul><li>clientIdentfier - the client identifier of the selected client</li><li>certHash - the hash of the certificate added to the selected client</li><li>certHashAlgorithm - the hash algorithm used to calculate value of the field certHash</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| Delete internal TLS certificate                          | <ul><li>clientIdentfier - the client identifier of the selected client</li><li>certHash - the hash of the certificate deleted from the selected client</li><li>certHashAlgorithm - the hash algorithm used to calculate value of the field certHash</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| Add group                                                | <ul><li>clientIdentifier - the client identifier of the selected client</li><li>groupCode - the code of the local group added to the selected client</li><li>groupDescription - the description of the added local group</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| Edit group description                                   | <ul><li>clientIdentifier - the client identifier of the selected client</li><li>groupCode - the code of the edited local group of the selected client</li><li>groupDescription - the new description of the edited local group</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| Add members to group                                     | <ul><li>clientIdentifier - the client identifier of the selected client</li><li>groupCode - the code of the selected local group of the selected client</li><li>memberIdentifiers - the list of member identifiers of members added to the selected local group</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| Remove members from group                                | <ul><li>clientIdentifier - the client identifier of the selected client</li><li>groupCode - the code of the selected global group of the selected client</li><li>memberIdentifiers - the list of member identifiers of the removed members</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| Delete group                                             | <ul><li>clientIdentifier - the client identifier of the selected client</li><li>groupCode - the code of the deleted local group of the selected client</li><li>groupDescription - the description of the deleted local group</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |

#### 2.2.4 System Parameters Events

The audit log events related to the system parameters.

| Event                                         | Data fields                                                                                                                                                                                                                                            |
|-----------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Generate certificate request for TLS**      | <ul><li>subjectName - the subject name of the generated certificate request</li></ul>                                                                                                                                                                  |
| **Import TLS certificate from file**          | <ul><li>certHash - the hash of the generated internal TLS certificate</li><li>certHashAlgorithm - the hash algorithm used to calculate value of the field certHash</li></ul>                                                                           |
| Upload configuration anchor                   | <ul><li>anchorFileHash - the hash of the uploaded anchor file</li><li>anchorFileHashAlgorithm - the hash algorithm used to calculate value of the field anchorFileHash</li><li>generatedAt - the UTC time when the anchor file was generated</li></ul> |
| Add timestamping service                      | <ul><li>tspName - the name of the added timestamping service</li><li>tspUrl - the URL of the added timestamping service</li></ul>                                                                                                                      |  
| Delete timestamping service                   | <ul><li>tspName - the name of the deleted timestamping service</li><li>tspUrl - the URL of the deleted timestamping service</li></ul>                                                                                                                  |
| Generate new internal TLS key and certificate | <ul><li>certHash - the hash of the generated internal TLS certificate</li><li>certHashAlgorithm - the hash algorithm used to calculate value of the field certHash</li></ul>                                                                           |

#### 2.2.5 Keys and Certificates Events

The audit log events related to keys and certificates management

| Event                                                                                                                                      | Data fields                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | 
|--------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Log in to token                                                                                                                            | <ul><li>tokenId - the identifier of the token logged in</li><li>tokenSerialNumber - the serial number of the token</li><li>tokenFriendlyName - the friendly name of the token</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| Log out from token                                                                                                                         | <ul><li>tokenId - the identifier of the token logged out</li><li>tokenSerialNumber - the serial number of the token</li><li>tokenFriendlyName - the friendly name of the token</li>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| Generate key                                                                                                                               | <ul><li>tokenId - the identifier of the token used to generate the key</li><li>tokenSerialNumber - the serial number of the token</li><li>tokenFriendlyName - the friendly name of the token</li><li>keyId - the identifier of the generated key</li><li>keyLabel - the label of the generated key</li><li>keyFriendlyName - the friendly name of the generated key</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| Delete key <br><br> Event name is used if event fails before *Delete key from token and configuration part* is reached                     | <ul><li>tokenId - the identifier of the token where the deleted key located</li><li>tokenSerialNumber - the serial number of the token</li><li>tokenFriendlyName - the friendly name of the token</li><li>keyId - the identifier of the deleted key</li><li>keyFriendlyName - the friendly name of the deleted key</li><li>keyUsage - the key usage of the deleted key</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| Delete key from token and configuration                                                                                                    | <ul><li>tokenId - the identifier of the token where the deleted key located</li><li>tokenSerialNumber - the serial number of the token</li><li>tokenFriendlyName - the friendly name of the token</li><li>keyId - the identifier of the deleted key</li><li>keyFriendlyName - the friendly name of the deleted key</li><li>keyUsage - the key usage of the deleted key</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| Generate CSR                                                                                                                               | <ul><li>tokenId - the identifier of the token used to generate the certificate request</li><li>tokenSerialNumber - the serial number of the token</li><li>tokenFriendlyName - the friendly name of the token</li><li>keyId - the identifier of the key used to generate the certificate request</li><li>keyFriendlyName - the friendly name of key</li><li>keyUsage - the key usage</li><li>clientIdentifier - the client identifier of the client which certificate request was generated</li><li>subjectName - the subject name of the generated certificate request</li><li>certificationServiceName - the name of the approved certification service for which the CSR was generated</li><li>csrFormat - the format (PEM / DER) of the generated CSR file</li></ul>                                                                                                                                       |
| Delete CSR                                                                                                                                 | <ul><li>tokenId - the identifier of the token where the key of the deleted certificate request located</li><li>tokenSerialNumber - the serial number of the token</li><li>tokenFriendlyName - the friendly name of the token</li><li>keyId - the identifier of the key related to the deleted certificate request</li><li>keyFriendlyName - the friendly name of the key</li><li>keyUsage - the key usage</li><li>csrId - the identifier of the deleted certificate request</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                         |
| Generate key and CSR                                                                                                                       | <ul><li>tokenId - the identifier of the token used to generate the key</li><li>tokenSerialNumber - the serial number of the token</li><li>tokenFriendlyName - the friendly name of the token</li><li>keyId - the identifier of the generated key</li><li>keyLabel - the label of the generated key</li><li>keyFriendlyName - the friendly name of the generated key</li><li>keyUsage - the key usage</li><li>clientIdentifier - the client identifier of the client which certificate request was generated</li><li>subjectName - the subject name of the generated certificate request</li><li>certificationServiceName - the name of the approved certification service for which the CSR was generated</li><li>csrFormat - the format (PEM / DER) of the generated CSR file</li></ul>                                                                                                                      |
| Import certificate from file                                                                                                               | <ul><li>certHash - the hash of the imported certificate file</li><li>certHashAlgorithm - the hash algorithm used to calculate value of the field certHash</li><li>keyUsage - the key usage of the imported certificate</li><li>clientIdentifier - the client identifier of the member constructed from signing certificate</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| Import certificate from token                                                                                                              | <ul><li>tokenId - identifier of the token where imported certificate located</li><li>tokenSerialNumber - the serial number of the token</li><li>tokenFriendlyName - the friendly name of the token</li><li>keyId - the identifier of the key related to the imported certificate</li><li>keyFriendlyName - the friendly name of the key</li><li>keyUsage - the key usage</li><li>certId - the identifier of the imported certificate</li><li>certHash - the hash of the imported certificate</li><li>certHashAlgorithm - the hash algorithm used to calculate value of the field certHash</li><li>clientIdentifier - the client identifier of the member constructed from signing certificate</li></ul>                                                                                                                                                                                                       |
| Delete certificate <br><br> Event name is used if event fails before it is known where certificate is delete from (configuration or token) |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| Delete certificate from configuration                                                                                                      | <ul><li>tokenId - the identifier of token where the key of the deleted certificate located</li><li>tokenSerialNumber - the serial number of the token</li><li>tokenFriendlyName - the friendly name of the token</li><li>keyId - the identifier of the key of the deleted certificate</li><li>keyFriendlyName - the friendly name of the key</li><li>keyUsage - the key usage</li><li>certId - the identifier of the deleted certificate</li><li>certHash - the hash of the deleted certificate</li><li>certHashAlgorithm - the hash algorithm used to calculate value of the field certHash</li></ul>                                                                                                                                                                                                                                                                                                        |
| Delete certificate from token                                                                                                              | <ul><li>tokenId - the identifier of token where the key of the deleted certificate located</li><li>tokenSerialNumber - the serial number of the token</li><li>tokenFriendlyName - the friendly name of the token</li><li>keyId - the identifier of the key of the deleted certificate</li><li>keyFriendlyName - the friendly name of the key</li><li>keyUsage - the key usage</li><li>certId - the identifier of the deleted certificate</li><li>certHash - the hash of the deleted certificate</li><li>certHashAlgorithm - the hash algorithm used to calculate value of the field certHash</li></ul>                                                                                                                                                                                                                                                                                                        |
| Enable certificate                                                                                                                         | <ul><li>tokenId - the identifier of token where the key of the enabled certificate located</li><li>tokenSerialNumber - the serial number of the token</li><li>tokenFriendlyName - the friendly name of the token</li><li>keyId - the identifier of the key of the enabled certificate</li><li>keyFriendlyName - the friendly name of the key</li><li>keyUsage - the key usage</li><li>certId - the identifier of the enabled certificate</li><li>certHash - the hash of the enabled certificate</li><li>certHashAlgorithm - the hash algorithm used to calculate value of the field certHash</li></ul>                                                                                                                                                                                                                                                                                                        |
| Disable certificate                                                                                                                        | <ul><li>tokenId - the identifier of the token where the key of the disabled certificate located</li><li>tokenSerialNumber - the serial number of the token</li><li>tokenFriendlyName - the friendly name of the token</li><li>keyId - the identifier of the key of the disabled certificate</li><li>keyFriendlyName - the friendly name of the key</li><li>keyUsage - the key usage</li><li>certId - the identifier of the disabled certificate</li><li>certHash - the hash of the disabled certificate</li><li>certHashAlgorithm - the hash algorithm used to calculate value of the field certHash</li></ul>                                                                                                                                                                                                                                                                                                |
| Register authentication certificate                                                                                                        | <ul><li>tokenId - the identifier of token where key of authentication certificate locates</li><li>tokenSerialNumber - the serial number of token where key of authentication certificate locates</li><li>tokenFriendlyName - the friendly name of token where key of authentication certificate locates</li><li>keyId - the identifier of key of registered authentication certificate</li><li>certId - the identifier of registered authentication certificate</li><li>certHash - the hash of registered authentication certificate</li><li>certHashAlgorithm - the hash algorithm used to calculate value of field certHash</li><li>address - the address of security server which authentication certificate was registered</li><li>managementRequestId - the identifier of the corresponding management request in the Central Server</li><li>certStatus - the status of registered certificate</li></ul> |
| Unregister authentication certificate                                                                                                      | <ul><li>tokenId - the identifier of the token where the key of the authentication certificate located</li><li>tokenSerialNumber - the serial number of the token</li><li>tokenFriendlyName - the friendly name of the token</li><li>keyId - the identifier of the key of the unregistered authentication certificate</li><li>certId - the identifier of the unregistered authentication certificate</li><li>certHash - the hash of the unregistered authentication certificate</li><li>certHashAlgorithm - the hash algorithm used to calculate value of the field certHash</li><li>managementRequestId - the identifier of the corresponding management request in the Central Server</li></ul><li>certStatus - the status of the unregistered certificate                                                                                                                                                   |
| Skip unregistration of authentication certificate                                                                                          | <ul><li>tokenId - the identifier of the token where the key of the authentication certificate located</li><li>tokenSerialNumber - the serial number of the token</li><li>tokenFriendlyName - the friendly name of the token</li><li>keyId - the identifier of the key of the unregistered authentication certificate</li><li>certId - the identifier of the unregistered authentication certificate</li><li>certHash - the hash of the unregistered authentication certificate</li><li>certHashAlgorithm - the hash algorithm used to calculate value of the field certHash</li><li>certStatus - the status of the unregistered certificate</li></ul>                                                                                                                                                                                                                                                         |
| Set friendly name to token                                                                                                                 | <ul><li>tokenId - the identifier of the selected token</li><li>tokenSerialNumber - the serial number of the selected token</li><li>tokenFriendlyName - the new friendly name of the selected token</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| Set friendly name to key                                                                                                                   | <ul><li>keyId - the identifier of the selected key</li><li>keyFriendlyName - the new friendly name of the selected key</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |

#### 2.2.6 Backup and Restore Events

The audit log events related to backup and restore.

| Event                 | Data fields                                                                                  |
|-----------------------|----------------------------------------------------------------------------------------------|
| Back up configuration | <ul><li>backupFileName - the name of the created backup file</li></ul>                       |
| Upload backup file    | <ul><li>backupFileName - the name of the uploaded backup file</li></ul>                      |
| Delete backup file    | <ul><li>backupFileName - the name of the deleted backup file</li></ul>                       |
| Restore configuration | <ul><li>backupFileName - the name of the backup file used to restore configuration</li></ul> |

#### 2.2.7 API Key Management Events

The audit log events related to API key management.

| Event          | Data fields                                                                                                                         |
|----------------|-------------------------------------------------------------------------------------------------------------------------------------|
| API key create | <ul><li>apiKeyId - identifier of the API key</li><li>apiKeyRoles - array containing the roles associated with the API key</li></ul> |
| API key update | <ul><li>apiKeyId - identifier of the API key</li><li>apiKeyRoles - array containing the roles associated with the API key</li></ul> |
| API key remove | <ul><li>apiKeyId - identifier of the API key</li><li>apiKeyRoles - array containing the roles associated with the API key</li></ul> |

#### 2.2.8 Technical Events

The audit log events related to technical events, such as authentication failures. Except for Key management API log in
event, these events are only logged if they fail.

| Event                                                                                                         | Data fields |
|---------------------------------------------------------------------------------------------------------------|-------------|
| Key management API log in                                                                                     |             |
| API key authentication                                                                                        |             |
| Auth credentials discovery                                                                                    |             |
| Access check <br><br> (if user did not have permission to do an operation which is not an audit logged event) |             |
| Authentication                                                                                                |             |

### 2.3 Utility signer-console

The audit log events logged by the utility signer-console.

| Event                                | Data fields                                                                                                                                                                                                                                                                                                                                                                               |
|--------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Set a friendly name to the token     | <ul><li>tokenId - the entered token identifier</li><li>tokenFriendlyName - the new friendly name for the entered token</li></ul>                                                                                                                                                                                                                                                          |
| Set a friendly name to the key       | <ul><li>keyId - the entered key identifier</li><li>keyFriendlyName - the new friendly name for the entered key</li></ul>                                                                                                                                                                                                                                                                  |
| Activate the certificate             | <ul><li>certId - the identifier of the activated certificate</li></ul>                                                                                                                                                                                                                                                                                                                    |
| Deactivate the certificate           | <ul><li>certId - the identifier of the deactivated certificate</li></ul>                                                                                                                                                                                                                                                                                                                  |
| Delete the key from token            | <ul><li>keyId - the identifier of the deleted key</li></ul>                                                                                                                                                                                                                                                                                                                               |
| Delete the certificate               | <ul><li>certId - the identifier of the deleted certificate</li></ul>                                                                                                                                                                                                                                                                                                                      |
| Delete the certificate request       | <ul><li>certRequestId - the identifier of the deleted certificate request</li></ul>                                                                                                                                                                                                                                                                                                       |
| Import a certificate from the file   | <ul><li>certFileName - the name of the imported certificate file</li><li>clientIdentifier - the client identifier of the member constructed from signing certificate</li><li>keyId - the identifier of the key to which the certificate was imported.</li></ul>                                                                                                                           |
| Log into the token                   | <ul><li>tokenId - the identifier of the token logged in</li></ul>                                                                                                                                                                                                                                                                                                                         |
| Initialize the software token        | <ul><li>tokenId - the identifier of the initialized token</li></ul>                                                                                                                                                                                                                                                                                                                       |
| Generate a key on the token          | <ul><li>tokenId - the identifier of the token used to generate the key</li><li>keyId - the identifier of the generated key</li><li>keyLabel - the label of the generated key</li></ul>                                                                                                                                                                                                    |
| Generate CSR                         | <ul><li>keyId - the identifier of the key used to generate the certification request</li><li>keyUsage - the key usage</li><li>clientIdentifier - the client identifier of the client which certificate request was generated</li><li>subjectName - the subject name of the generated certification request</li><li>csrFormat - the format (PEM / DER) of the generated CSR file</li></ul> |
