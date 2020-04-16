---
title: <specifiedPickupDirectory>要素 (ネットワーク設定)
ms.date: 03/30/2017
f1_keywords:
- http://schemas.microsoft.com/.NetConfiguration/v2.0#specifiedPickupDirectory
- http://schemas.microsoft.com/.NetConfiguration/v2.0#configuration/system.net/mailSettings/smtp/specifiedPickupDirectory
helpviewer_keywords:
- specifiedPickupDirectory element
- <specifiedPickupDirectory> element
ms.assetid: 0121f49d-bff2-4bc6-af06-f1628dcd61f1
ms.openlocfilehash: 0d9c68f887edd33d91c894a3caa47e37132dcd5c
ms.sourcegitcommit: 1f954dcf7d4bb347970c326ed6197d8bfdd38aea
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2020
ms.locfileid: "6613092"
---
# <a name="specifiedpickupdirectory-element-network-settings"></a>\<設定の候補ディレクトリ> 要素 (ネットワーク設定)
簡易メール転送プロトコル (SMTP) サーバーのローカルディレクトリを構成します。  
  
[**\<構成>**](../configuration-element.md)\
&nbsp;&nbsp;[**\<system.net>**](system-net-element-network-settings.md)\
&nbsp;&nbsp;&nbsp;&nbsp;[**\<mailSettings>**](mailsettings-element-network-settings.md)\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[**\<smtp>**](smtp-element-network-settings.md)\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**\<>の候補ディレクトリの**  
  
## <a name="syntax"></a>引数  
  
```xml  
<specifiedPickupDirectory  
  pickupDirectoryLocation="directory"
/>  
```  
  
## <a name="attributes-and-elements"></a>属性と要素  
 以下のセクションでは、属性、子要素、および親要素について説明します。  
  
### <a name="attributes"></a>属性  
  
|属性|説明|  
|---------------|-----------------|  
|`pickupDirectoryLocation`|後で SMTP サーバーで処理するために、アプリケーションがメールを保存するディレクトリ。|  
  
### <a name="child-elements"></a>子要素  
 -.  
  
### <a name="parent-elements"></a>親要素  
  
|オブジェクト|説明|  
|-------------|-----------------|  
|[\<smtp> 要素 (ネットワーク設定)](smtp-element-network-settings.md)|簡易メール転送プロトコル (SMTP) のメール送信オプションを構成します。|  
  
## <a name="remarks"></a>終わり  
 この`specifiedPickupDirectory`属性は、SMTP サーバーによって処理されるメールメッセージをアプリケーションが保存するディレクトリを設定します。  
  
## <a name="example"></a>次  
 次の例では、メールピックアップディレクトリとして c:\ メールを指定しています。  
  
```xml  
<configuration>  
  <system.net>  
    <mailSettings>  
      <smtp deliveryMethod="SpecifiedPickupDirectory">  
        <specifiedPickupDirectory  
          pickupDirectoryLocation="c:\maildrop"  
        />  
      </smtp>  
    </mailSettings>  
  </system.net>  
</configuration>  
```  
  
## <a name="see-also"></a>関連項目

- <xref:System.Net.Mail.SmtpClient?displayProperty=nameWithType>
- <xref:System.Net.Configuration.SmtpSection?displayProperty=nameWithType>
- <xref:System.Net.Configuration.SmtpSpecifiedPickupDirectoryElement?displayProperty=nameWithType>
- [ネットワーク設定スキーマ](index.md)