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
ms.sourcegitcommit: 7335c82f5336142f6bb802210d8c7e2736a4c022
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2020
ms.locfileid: "6613566"
---
# <a name="specifiedpickupdirectory-element-network-settings"></a><span data-ttu-id="d7d06-102">\<specifiedPickupDirectory>要素 (ネットワーク設定)</span><span class="sxs-lookup"><span data-stu-id="d7d06-102">\<specifiedPickupDirectory> Element (Network Settings)</span></span>
<span data-ttu-id="d7d06-103">簡易メール転送プロトコル (SMTP) サーバーのローカルディレクトリを構成します。</span><span class="sxs-lookup"><span data-stu-id="d7d06-103">Configures the local directory for a Simple Mail Transport Protocol (SMTP) server.</span></span>  
  
[**\<configuration>**](../configuration-element.md)\
&nbsp;&nbsp;[**\<system.net>**](system-net-element-network-settings.md)\
&nbsp;&nbsp;&nbsp;&nbsp;[**\<mailSettings>**](mailsettings-element-network-settings.md)\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[**\<smtp>**](smtp-element-network-settings.md)\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**\<specifiedPickupDirectory>**  
  
## <a name="syntax"></a><span data-ttu-id="d7d06-104">引数</span><span class="sxs-lookup"><span data-stu-id="d7d06-104">Syntax</span></span>  
  
```xml  
<specifiedPickupDirectory  
  pickupDirectoryLocation="directory"
/>  
```  
  
## <a name="attributes-and-elements"></a><span data-ttu-id="d7d06-105">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d7d06-105">Attributes and Elements</span></span>  
 <span data-ttu-id="d7d06-106">以下のセクションでは、属性、子要素、および親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d7d06-106">The following sections describe attributes, child elements, and parent elements.</span></span>  
  
### <a name="attributes"></a><span data-ttu-id="d7d06-107">属性</span><span class="sxs-lookup"><span data-stu-id="d7d06-107">Attributes</span></span>  
  
|<span data-ttu-id="d7d06-108">属性</span><span class="sxs-lookup"><span data-stu-id="d7d06-108">Attribute</span></span>|<span data-ttu-id="d7d06-109">説明</span><span class="sxs-lookup"><span data-stu-id="d7d06-109">Description</span></span>|  
|---------------|-----------------|  
|`pickupDirectoryLocation`|<span data-ttu-id="d7d06-110">後で SMTP サーバーで処理するために、アプリケーションがメールを保存するディレクトリ。</span><span class="sxs-lookup"><span data-stu-id="d7d06-110">The directory where applications save email for later processing by the SMTP server.</span></span>|  
  
### <a name="child-elements"></a><span data-ttu-id="d7d06-111">子要素</span><span class="sxs-lookup"><span data-stu-id="d7d06-111">Child Elements</span></span>  
 <span data-ttu-id="d7d06-112">-.</span><span class="sxs-lookup"><span data-stu-id="d7d06-112">None.</span></span>  
  
### <a name="parent-elements"></a><span data-ttu-id="d7d06-113">親要素</span><span class="sxs-lookup"><span data-stu-id="d7d06-113">Parent Elements</span></span>  
  
|<span data-ttu-id="d7d06-114">オブジェクト</span><span class="sxs-lookup"><span data-stu-id="d7d06-114">Element</span></span>|<span data-ttu-id="d7d06-115">説明</span><span class="sxs-lookup"><span data-stu-id="d7d06-115">Description</span></span>|  
|-------------|-----------------|  
|[<span data-ttu-id="d7d06-116">\<smtp>要素 (ネットワーク設定)</span><span class="sxs-lookup"><span data-stu-id="d7d06-116">\<smtp> Element (Network Settings)</span></span>](smtp-element-network-settings.md)|<span data-ttu-id="d7d06-117">簡易メール転送プロトコル (SMTP) のメール送信オプションを構成します。</span><span class="sxs-lookup"><span data-stu-id="d7d06-117">Configures Simple Mail Transport Protocol (SMTP) mail sending options.</span></span>|  
  
## <a name="remarks"></a><span data-ttu-id="d7d06-118">終わり</span><span class="sxs-lookup"><span data-stu-id="d7d06-118">Remarks</span></span>  
 <span data-ttu-id="d7d06-119">この`specifiedPickupDirectory`属性は、SMTP サーバーによって処理されるメールメッセージをアプリケーションが保存するディレクトリを設定します。</span><span class="sxs-lookup"><span data-stu-id="d7d06-119">The `specifiedPickupDirectory` attribute sets the directory where applications save mail messages to be processed by the SMTP server.</span></span>  
  
## <a name="example"></a><span data-ttu-id="d7d06-120">次</span><span class="sxs-lookup"><span data-stu-id="d7d06-120">Example</span></span>  
 <span data-ttu-id="d7d06-121">次の例では、メールピックアップディレクトリとして c:\ メールを指定しています。</span><span class="sxs-lookup"><span data-stu-id="d7d06-121">The following example specifies c:\maildrop as the mail pickup directory.</span></span>  
  
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
  
## <a name="see-also"></a><span data-ttu-id="d7d06-122">関連項目</span><span class="sxs-lookup"><span data-stu-id="d7d06-122">See also</span></span>

- <xref:System.Net.Mail.SmtpClient?displayProperty=nameWithType>
- <xref:System.Net.Configuration.SmtpSection?displayProperty=nameWithType>
- <xref:System.Net.Configuration.SmtpSpecifiedPickupDirectoryElement?displayProperty=nameWithType>
- [<span data-ttu-id="d7d06-123">ネットワーク設定スキーマ</span><span class="sxs-lookup"><span data-stu-id="d7d06-123">Network Settings Schema</span></span>](index.md)