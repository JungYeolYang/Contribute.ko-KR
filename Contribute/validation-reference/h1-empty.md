---
title: h1-empty
description: Docs 빌드 문제 h1-empty에 대한 설명 및 해결 방법.
author: meganbradley
ms.author: mbradley
ms.topic: error-reference
ms.date: 12/12/2018
ms.prod: non-product-specific
ms.openlocfilehash: bb07235f7cd1ba6d45418c48a4190255bdd9a428
ms.sourcegitcommit: 4053577bd0478d711257a283ee661d618b49c2df
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/05/2019
ms.locfileid: "57427687"
---
# <a name="h1-empty"></a><span data-ttu-id="296c3-103">h1-empty</span><span class="sxs-lookup"><span data-stu-id="296c3-103">h1-empty</span></span>

## <a name="warning"></a><span data-ttu-id="296c3-104">경고</span><span class="sxs-lookup"><span data-stu-id="296c3-104">Warning</span></span>

`H1 is required. Add content to your top-level heading.`

<span data-ttu-id="296c3-105">H1은 Markdown 파일의 첫 번째 제목을 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="296c3-105">H1 refers to the first heading in a Markdown file.</span></span> <span data-ttu-id="296c3-106">docs.microsoft.com에 게시하면 H1이 페이지 맨 위에 큰 글꼴로 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="296c3-106">When published to docs.microsoft.com, the H1 shows at the top of the page in a large font.</span></span> <span data-ttu-id="296c3-107">H1은 단일 해시(#), 공백 및 제목 텍스트를 차례로 사용하는 행을 시작하여 작성됩니다.</span><span class="sxs-lookup"><span data-stu-id="296c3-107">An H1 is created by beginning a line with a single hash (#) followed by a space, then the heading text.</span></span>

## <a name="resolution"></a><span data-ttu-id="296c3-108">해결 방법</span><span class="sxs-lookup"><span data-stu-id="296c3-108">Resolution</span></span>

<span data-ttu-id="296c3-109">이 문제를 해결하려면 H1에 해시뿐 아니라 콘텐츠도 포함되어 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="296c3-109">To fix this issue, make sure your H1 includes content, not just a hash.</span></span>

<span data-ttu-id="296c3-110">나쁨:</span><span class="sxs-lookup"><span data-stu-id="296c3-110">Bad:</span></span>

```markdown
---
author: meganbradley
ms.author: mbradley
---
#
This is not an H1
```

<span data-ttu-id="296c3-111">좋음:</span><span class="sxs-lookup"><span data-stu-id="296c3-111">Good:</span></span>

```markdown
---
author: meganbradley
ms.author: mbradley
---
# This is an H1
```

<!--make sure to add this file to your includes folder and verify the path-->
[!INCLUDE [validation-reference-help](includes/validation-reference-help.md)]