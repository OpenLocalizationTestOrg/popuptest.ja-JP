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
# <a name="update-test-on-june-23"></a><span data-ttu-id="d1975-102">更新テスト (6 月23日)</span><span class="sxs-lookup"><span data-stu-id="d1975-102">Update test on June 23</span></span>
  
# <a name="specifiedpickupdirectory-element-network-settings"></a><span data-ttu-id="d1975-103">\<specifiedPickupDirectory>要素 (ネットワーク設定)</span><span class="sxs-lookup"><span data-stu-id="d1975-103">\<specifiedPickupDirectory> Element (Network Settings)</span></span>
<span data-ttu-id="d1975-104">簡易メール転送プロトコル (SMTP) サーバーのローカルディレクトリを構成します。</span><span class="sxs-lookup"><span data-stu-id="d1975-104">Configures the local directory for a Simple Mail Transport Protocol (SMTP) server.</span></span>  
  
[**\<configuration>**](../configuration-element.md)\
&nbsp;&nbsp;[**\<system.net>**](system-net-element-network-settings.md)\
&nbsp;&nbsp;&nbsp;&nbsp;[**\<mailSettings>**](mailsettings-element-network-settings.md)\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[**\<smtp>**](smtp-element-network-settings.md)\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**\<specifiedPickupDirectory>**  
  
## <a name="syntax"></a><span data-ttu-id="d1975-105">引数</span><span class="sxs-lookup"><span data-stu-id="d1975-105">Syntax</span></span>  
  
```xml  
<specifiedPickupDirectory  
  pickupDirectoryLocation="directory"
/>  
```  
  
## <a name="attributes-and-elements"></a><span data-ttu-id="d1975-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d1975-106">Attributes and Elements</span></span>  
 <span data-ttu-id="d1975-107">以下のセクションでは、属性、子要素、および親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d1975-107">The following sections describe attributes, child elements, and parent elements.</span></span>  
  
### <a name="attributes"></a><span data-ttu-id="d1975-108">属性</span><span class="sxs-lookup"><span data-stu-id="d1975-108">Attributes</span></span>  
  
|<span data-ttu-id="d1975-109">属性</span><span class="sxs-lookup"><span data-stu-id="d1975-109">Attribute</span></span>|<span data-ttu-id="d1975-110">説明</span><span class="sxs-lookup"><span data-stu-id="d1975-110">Description</span></span>|  
|---------------|-----------------|  
|`pickupDirectoryLocation`|<span data-ttu-id="d1975-111">後で SMTP サーバーで処理するために、アプリケーションがメールを保存するディレクトリ。</span><span class="sxs-lookup"><span data-stu-id="d1975-111">The directory where applications save email for later processing by the SMTP server.</span></span>|  
  
### <a name="child-elements"></a><span data-ttu-id="d1975-112">子要素</span><span class="sxs-lookup"><span data-stu-id="d1975-112">Child Elements</span></span>  
 <span data-ttu-id="d1975-113">-.</span><span class="sxs-lookup"><span data-stu-id="d1975-113">None.</span></span>  
  
### <a name="parent-elements"></a><span data-ttu-id="d1975-114">親要素</span><span class="sxs-lookup"><span data-stu-id="d1975-114">Parent Elements</span></span>  
  
|<span data-ttu-id="d1975-115">オブジェクト</span><span class="sxs-lookup"><span data-stu-id="d1975-115">Element</span></span>|<span data-ttu-id="d1975-116">説明</span><span class="sxs-lookup"><span data-stu-id="d1975-116">Description</span></span>|  
|-------------|-----------------|  
|[<span data-ttu-id="d1975-117">\<smtp>要素 (ネットワーク設定)</span><span class="sxs-lookup"><span data-stu-id="d1975-117">\<smtp> Element (Network Settings)</span></span>](smtp-element-network-settings.md)|<span data-ttu-id="d1975-118">簡易メール転送プロトコル (SMTP) のメール送信オプションを構成します。</span><span class="sxs-lookup"><span data-stu-id="d1975-118">Configures Simple Mail Transport Protocol (SMTP) mail sending options.</span></span>|  
  
## <a name="remarks"></a><span data-ttu-id="d1975-119">終わり</span><span class="sxs-lookup"><span data-stu-id="d1975-119">Remarks</span></span>  
 <span data-ttu-id="d1975-120">この `specifiedPickupDirectory` 属性は、SMTP サーバーによって処理されるメールメッセージをアプリケーションが保存するディレクトリを設定します。</span><span class="sxs-lookup"><span data-stu-id="d1975-120">The `specifiedPickupDirectory` attribute sets the directory where applications save mail messages to be processed by the SMTP server.</span></span>  
  
## <a name="example"></a><span data-ttu-id="d1975-121">次</span><span class="sxs-lookup"><span data-stu-id="d1975-121">Example</span></span>  
 <span data-ttu-id="d1975-122">次の例では、メールピックアップディレクトリとして c:\ メールを指定しています。</span><span class="sxs-lookup"><span data-stu-id="d1975-122">The following example specifies c:\maildrop as the mail pickup directory.</span></span>  
  
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
  
## <a name="see-also"></a><span data-ttu-id="d1975-123">関連項目</span><span class="sxs-lookup"><span data-stu-id="d1975-123">See also</span></span>

- <xref:System.Net.Mail.SmtpClient?displayProperty=nameWithType>
- <xref:System.Net.Configuration.SmtpSection?displayProperty=nameWithType>
- <xref:System.Net.Configuration.SmtpSpecifiedPickupDirectoryElement?displayProperty=nameWithType>
- [<span data-ttu-id="d1975-124">ネットワーク設定スキーマ</span><span class="sxs-lookup"><span data-stu-id="d1975-124">Network Settings Schema</span></span>](index.md)
