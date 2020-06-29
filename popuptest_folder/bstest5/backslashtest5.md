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
ms.openlocfilehash: 25b06619a91e43d54b92c1e2cc50b433ccf864bc
ms.sourcegitcommit: e25a89331cdb027dcfc845e774571df86e62dcb2
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2020
ms.locfileid: "6614896"
---
# <a name="update-test-on-june-23"></a>更新テスト (6 月23日)
  
# <a name="specifiedpickupdirectory-element-network-settings"></a>\<specifiedPickupDirectory>要素 (ネットワーク設定)
簡易メール転送プロトコル (SMTP) サーバーのローカルディレクトリを構成します。  
  
[**\<configuration>**](../configuration-element.md)\
&nbsp;&nbsp;[**\<system.net>**](system-net-element-network-settings.md)\
&nbsp;&nbsp;&nbsp;&nbsp;[**\<mailSettings>**](mailsettings-element-network-settings.md)\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[**\<smtp>**](smtp-element-network-settings.md)\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**\<specifiedPickupDirectory>**  
  
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
|[\<smtp>要素 (ネットワーク設定)](smtp-element-network-settings.md)|簡易メール転送プロトコル (SMTP) のメール送信オプションを構成します。|  
  
## <a name="remarks"></a>終わり  
 この `specifiedPickupDirectory` 属性は、SMTP サーバーによって処理されるメールメッセージをアプリケーションが保存するディレクトリを設定します。  
  
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
