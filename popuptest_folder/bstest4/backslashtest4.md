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
# <a name="specifiedpickupdirectory-element-network-settings"></a><span data-ttu-id="92c72-102">\<設定の候補ディレクトリ> 要素 (ネットワーク設定)</span><span class="sxs-lookup"><span data-stu-id="92c72-102">\<specifiedPickupDirectory> Element (Network Settings)</span></span>
<span data-ttu-id="92c72-103">簡易メール転送プロトコル (SMTP) サーバーのローカルディレクトリを構成します。</span><span class="sxs-lookup"><span data-stu-id="92c72-103">Configures the local directory for a Simple Mail Transport Protocol (SMTP) server.</span></span>  
  
<span data-ttu-id="92c72-104">[**\<構成>**](../configuration-element.md)</span><span class="sxs-lookup"><span data-stu-id="92c72-104">[**\<configuration>**](../configuration-element.md)</span></span>\
<span data-ttu-id="92c72-105">&nbsp;&nbsp;[**\<system.net>**](system-net-element-network-settings.md)</span><span class="sxs-lookup"><span data-stu-id="92c72-105">&nbsp;&nbsp;[**\<system.net>**](system-net-element-network-settings.md)</span></span>\
<span data-ttu-id="92c72-106">&nbsp;&nbsp;&nbsp;&nbsp;[**\<mailSettings>**](mailsettings-element-network-settings.md)</span><span class="sxs-lookup"><span data-stu-id="92c72-106">&nbsp;&nbsp;&nbsp;&nbsp;[**\<mailSettings>**](mailsettings-element-network-settings.md)</span></span>\
<span data-ttu-id="92c72-107">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[**\<smtp>**](smtp-element-network-settings.md)</span><span class="sxs-lookup"><span data-stu-id="92c72-107">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[**\<smtp>**](smtp-element-network-settings.md)</span></span>\
<span data-ttu-id="92c72-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**\<>の候補ディレクトリの**</span><span class="sxs-lookup"><span data-stu-id="92c72-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**\<specifiedPickupDirectory>**</span></span>  
  
## <a name="syntax"></a><span data-ttu-id="92c72-109">引数</span><span class="sxs-lookup"><span data-stu-id="92c72-109">Syntax</span></span>  
  
```xml  
<specifiedPickupDirectory  
  pickupDirectoryLocation="directory"
/>  
```  
  
## <a name="attributes-and-elements"></a><span data-ttu-id="92c72-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="92c72-110">Attributes and Elements</span></span>  
 <span data-ttu-id="92c72-111">以下のセクションでは、属性、子要素、および親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="92c72-111">The following sections describe attributes, child elements, and parent elements.</span></span>  
  
### <a name="attributes"></a><span data-ttu-id="92c72-112">属性</span><span class="sxs-lookup"><span data-stu-id="92c72-112">Attributes</span></span>  
  
|<span data-ttu-id="92c72-113">属性</span><span class="sxs-lookup"><span data-stu-id="92c72-113">Attribute</span></span>|<span data-ttu-id="92c72-114">説明</span><span class="sxs-lookup"><span data-stu-id="92c72-114">Description</span></span>|  
|---------------|-----------------|  
|`pickupDirectoryLocation`|<span data-ttu-id="92c72-115">後で SMTP サーバーで処理するために、アプリケーションがメールを保存するディレクトリ。</span><span class="sxs-lookup"><span data-stu-id="92c72-115">The directory where applications save email for later processing by the SMTP server.</span></span>|  
  
### <a name="child-elements"></a><span data-ttu-id="92c72-116">子要素</span><span class="sxs-lookup"><span data-stu-id="92c72-116">Child Elements</span></span>  
 <span data-ttu-id="92c72-117">-.</span><span class="sxs-lookup"><span data-stu-id="92c72-117">None.</span></span>  
  
### <a name="parent-elements"></a><span data-ttu-id="92c72-118">親要素</span><span class="sxs-lookup"><span data-stu-id="92c72-118">Parent Elements</span></span>  
  
|<span data-ttu-id="92c72-119">オブジェクト</span><span class="sxs-lookup"><span data-stu-id="92c72-119">Element</span></span>|<span data-ttu-id="92c72-120">説明</span><span class="sxs-lookup"><span data-stu-id="92c72-120">Description</span></span>|  
|-------------|-----------------|  
|[<span data-ttu-id="92c72-121">\<smtp> 要素 (ネットワーク設定)</span><span class="sxs-lookup"><span data-stu-id="92c72-121">\<smtp> Element (Network Settings)</span></span>](smtp-element-network-settings.md)|<span data-ttu-id="92c72-122">簡易メール転送プロトコル (SMTP) のメール送信オプションを構成します。</span><span class="sxs-lookup"><span data-stu-id="92c72-122">Configures Simple Mail Transport Protocol (SMTP) mail sending options.</span></span>|  
  
## <a name="remarks"></a><span data-ttu-id="92c72-123">終わり</span><span class="sxs-lookup"><span data-stu-id="92c72-123">Remarks</span></span>  
 <span data-ttu-id="92c72-124">この`specifiedPickupDirectory`属性は、SMTP サーバーによって処理されるメールメッセージをアプリケーションが保存するディレクトリを設定します。</span><span class="sxs-lookup"><span data-stu-id="92c72-124">The `specifiedPickupDirectory` attribute sets the directory where applications save mail messages to be processed by the SMTP server.</span></span>  
  
## <a name="example"></a><span data-ttu-id="92c72-125">次</span><span class="sxs-lookup"><span data-stu-id="92c72-125">Example</span></span>  
 <span data-ttu-id="92c72-126">次の例では、メールピックアップディレクトリとして c:\ メールを指定しています。</span><span class="sxs-lookup"><span data-stu-id="92c72-126">The following example specifies c:\maildrop as the mail pickup directory.</span></span>  
  
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
  
## <a name="see-also"></a><span data-ttu-id="92c72-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="92c72-127">See also</span></span>

- <xref:System.Net.Mail.SmtpClient?displayProperty=nameWithType>
- <xref:System.Net.Configuration.SmtpSection?displayProperty=nameWithType>
- <xref:System.Net.Configuration.SmtpSpecifiedPickupDirectoryElement?displayProperty=nameWithType>
- [<span data-ttu-id="92c72-128">ネットワーク設定スキーマ</span><span class="sxs-lookup"><span data-stu-id="92c72-128">Network Settings Schema</span></span>](index.md)