---
title: OPS 및 docs.microsoft.com에 대한 Markdown 참조
description: Markdown 및 DFM(DocFX Flavored Markdown) 확장에 대한 OPS 플랫폼 가이드입니다.
author: meganbradley
ms.author: mbradley
manager: jemash
ms.date: 05/18/2018
ms.topic: contributor-guide
ms.prod: non-product-specific
audience: internal,external
ms.openlocfilehash: e248eafb0247b200313ba198f2545eca947f5627
ms.sourcegitcommit: d3c7b49dc854dae8da9cd49da8ac4035789a5010
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/23/2018
ms.locfileid: "49805908"
---
# <a name="markdown-reference-for-ops"></a><span data-ttu-id="c8772-103">OPS에 대한 Markdown 참조</span><span class="sxs-lookup"><span data-stu-id="c8772-103">Markdown Reference for OPS</span></span>

<span data-ttu-id="c8772-104">Markdown은 일반 텍스트 서식 구문을 사용하는 경량 생성 언어입니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-104">Markdown is a lightweight markup language with plain text formatting syntax.</span></span> <span data-ttu-id="c8772-105">OPS는 Markdown에 대한 CommonMark 표준과 docs.microsoft.com에서 더 풍부한 콘텐츠를 제공하도록 설계된 사용자 지정 Markdown 확장을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-105">OPS supports the CommonMark standard for Markdown, plus some custom Markdown extensions designed to provide richer content on docs.microsoft.com.</span></span> <span data-ttu-id="c8772-106">이 문서에서는 OPS에서 docs.microsoft.com에 대해 Markdown을 사용하기 위한 사전순 참조를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-106">This article provides an alphabetical reference for using Markdown in OPS for docs.microsoft.com.</span></span>

<span data-ttu-id="c8772-107">텍스트 편집기를 사용하여 Markdown을 작성할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-107">You can use any text editor to author Markdown.</span></span> <span data-ttu-id="c8772-108">표준 Markdown 구문과 사용자 지정 OPS 확장을 쉽게 삽입할 수 있는 편집기의 경우 [Docs Authoring Pack](https://aka.ms/DocsAuthoringPack)이 설치된 [VS Code](https://code.visualstudio.com/)를 사용하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-108">For an editor that facilitates inserting both standard Markdown syntax and custom OPS extensions, we recommend [VS Code](https://code.visualstudio.com/) with the [Docs Authoring Pack](https://aka.ms/DocsAuthoringPack) installed.</span></span>

<span data-ttu-id="c8772-109">OPS는 모든 새로운 리포지토리를 위해 Markdig에서 표준화했으며, 이전 리포지토리는 Markdig로 마이그레이션하고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-109">OPS has standardized on Markdig for all new repos, and older repos are migrating to Markdig.</span></span> <span data-ttu-id="c8772-110">[https://babelmark.github.io/](https://babelmark.github.io/)에서 Markdig 및 기타 엔진에 대한 Markdown의 렌더링을 테스트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-110">You can test the rendering of Markdown in Markdig vs. other engines at [https://babelmark.github.io/](https://babelmark.github.io/).</span></span>

## <a name="alerts-note-tip-important-caution-warning"></a><span data-ttu-id="c8772-111">경고(alert)(참고, 팁, 중요, 주의, 경고(warning))</span><span class="sxs-lookup"><span data-stu-id="c8772-111">Alerts (Note, Tip, Important, Caution, Warning)</span></span>

<span data-ttu-id="c8772-112">OPS 관련 Markdown 확장을 경고하여 docs.microsoft.com에서 콘텐츠의 중요도를 색과 아이콘으로 표시하여 렌더링하는 블록 따옴표를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-112">Alerts an OPS-specific Markdown extension to create block quotes that render on docs.microsoft.com with colors and icons that indicate the significance of the content.</span></span> <span data-ttu-id="c8772-113">다음과 같은 경고 유형이 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-113">The following alert types are supported:</span></span>

```markdown
> [!NOTE]
> Information the user should notice even if skimming.

> [!TIP]
> Optional information to help a user be more successful.

> [!IMPORTANT]
> Essential information required for user success.

> [!CAUTION]
> Negative potential consequences of an action.

> [!WARNING]
> Dangerous certain consequences of an action.
```

<span data-ttu-id="c8772-114">이러한 경고는 docs.microsoft.com에서 다음과 같이 보입니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-114">These alerts look like this on docs.microsoft.com:</span></span>

> [!NOTE]
> <span data-ttu-id="c8772-115">훑어보더라도 사용자가 주목해야 할 정보입니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-115">Information the user should notice even if skimming.</span></span>

> [!TIP]
> <span data-ttu-id="c8772-116">사용자의 성공을 돕기 위한 선택적 정보입니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-116">Optional information to help a user be more successful.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c8772-117">사용자 성공을 위해 필요한 필수 정보입니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-117">Essential information required for user success.</span></span>

> [!CAUTION]
> <span data-ttu-id="c8772-118">작업의 잠재적인 부정적인 결과입니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-118">Negative potential consequences of an action.</span></span>

> [!WARNING]
> <span data-ttu-id="c8772-119">작업의 위험한 특정 결과입니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-119">Dangerous certain consequences of an action.</span></span>

## <a name="code-snippets"></a><span data-ttu-id="c8772-120">코드 조각</span><span class="sxs-lookup"><span data-stu-id="c8772-120">Code snippets</span></span>

<span data-ttu-id="c8772-121">Markdown 파일에 코드 조각을 포함할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-121">You can embed code snippets in your Markdown files:</span></span>

```markdown
[!code-<language>[<name>](<codepath><queryoption><queryoptionvalue> "<title>")]
```

## <a name="headings"></a><span data-ttu-id="c8772-122">제목</span><span class="sxs-lookup"><span data-stu-id="c8772-122">Headings</span></span>

<span data-ttu-id="c8772-123">OPS는 6가지 수준의 Markdown 제목을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-123">OPS supports six levels of Markdown headings:</span></span>

```markdown
# This is a first level heading (H1)

## This is a second level heading (H2)

...

###### This is a sixth level heading (H6)
```

- <span data-ttu-id="c8772-124">마지막 `#`과 제목 텍스트 사이에는 공백이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-124">There must be a space between the last `#` and heading text.</span></span>
- <span data-ttu-id="c8772-125">각 Markdown 파일에는 H1이 하나만 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-125">Each Markdown file must have one and only one H1.</span></span>
- <span data-ttu-id="c8772-126">H1은 파일에서 YML 메타데이터 블록 다음의 첫 번째 콘텐츠여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-126">The H1 must be the first content in the file after the YML metadata block.</span></span>
- <span data-ttu-id="c8772-127">H2는 게시된 파일의 오른쪽 탐색 메뉴에 자동으로 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-127">H2s automatically appear in the right-hand navigating menu of the published file.</span></span> <span data-ttu-id="c8772-128">하위 수준의 제목은 그렇지 않으므로 H2를 전략적으로 사용하여 독자가 콘텐츠를 탐색하는 것을 돕습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-128">Lower-level headings do not, so use H2s strategically to help readers navigate your content.</span></span>
- <span data-ttu-id="c8772-129">`<h1>`과 같은 HTML 제목은 권장되지 않으며 경우에 따라 빌드 경고가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-129">HMTL headings, such as `<h1>`, are not recommended and in some cases will cause build warnings.</span></span>
- <span data-ttu-id="c8772-130">[책갈피](#bookmark-links)를 통해 파일의 개별 제목에 연결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-130">You can link to individual headings in a file via [bookmarks](#bookmark-links).</span></span>

## <a name="html"></a><span data-ttu-id="c8772-131">HTML</span><span class="sxs-lookup"><span data-stu-id="c8772-131">HTML</span></span>

<span data-ttu-id="c8772-132">Markdown은 인라인 HTML을 지원하지만 HTML은 OPS를 통한 게시에는 권장되지 않으며 제한된 값 목록을 제외하고는 빌드 오류 또는 경고가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-132">Although Markdown supports inline HTML, HTML is not recommended for publishing via OPS, and except for a limited list of values will cause build errors or warnings.</span></span> <!--For more information, see HTML Whitelist. // do we want to add the whitelist? -->

## <a name="images"></a><span data-ttu-id="c8772-133">이미지</span><span class="sxs-lookup"><span data-stu-id="c8772-133">Images</span></span>

<span data-ttu-id="c8772-134">이미지를 포함하는 구문은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-134">The syntax to include an image is:</span></span>

```markdown
![[alt text]](<folderPath>)

Example:
![alt text for image](../images/Introduction.png)
```

<span data-ttu-id="c8772-135">여기서 `alt text`는 이미지에 대한 간략한 설명이고 `<folder path>`는 이미지에 대한 상대 경로입니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-135">Where `alt text` is a brief description of the image and `<folder path>` is a relative path to the image.</span></span> <span data-ttu-id="c8772-136">시각 장애인용 화면 읽기 프로그램에는 대체 텍스트가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-136">Alternate text is required for screen readers for the visually impaired.</span></span> <span data-ttu-id="c8772-137">또한 이미지를 렌더링할 수 없는 사이트 버그가 있는 경우에도 유용합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-137">It is also useful if there is a site bug where the image cannot render.</span></span>

<span data-ttu-id="c8772-138">이미지는 문서 집합 내의 `/media` 폴더에 저장해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-138">Images should be stored in a `/media` folder within your doc set.</span></span> <span data-ttu-id="c8772-139">기본적으로 이미지에 대해 다음 파일 형식이 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-139">The following file types are supported by default for images:</span></span>

- <span data-ttu-id="c8772-140">.jpg</span><span class="sxs-lookup"><span data-stu-id="c8772-140">.jpg</span></span>
- <span data-ttu-id="c8772-141">.png</span><span class="sxs-lookup"><span data-stu-id="c8772-141">.png</span></span>

<span data-ttu-id="c8772-142">문서 집합에 대한 docfx.json 파일<!--add link to reference when available-->에 리소스로 추가하여 다른 이미지 형식에 대한 지원을 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-142">You can add support for other image types by adding them as resources to the docfx.json file<!--add link to reference when available--> for your doc set.</span></span>

## <a name="links"></a><span data-ttu-id="c8772-143">링크</span><span class="sxs-lookup"><span data-stu-id="c8772-143">Links</span></span>

<span data-ttu-id="c8772-144">대부분의 경우 OPS는 다른 파일 및 페이지에 대한 표준 Markdown 링크를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-144">In most cases, OPS uses standard Markdown links to other files and pages.</span></span> <span data-ttu-id="c8772-145">링크 유형은 아래의 하위 섹션에서 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-145">The types of links are described in subsections below.</span></span>

> [!TIP]
> <span data-ttu-id="c8772-146">VS Code용 Docs Authoring Pack은 경로를 찾는 번거로움 없이 상대 링크와 책갈피를 올바르게 삽입하는 데 도움을 줄 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-146">The Docs Authoring Pack for VS Code can help insert relative links and bookmarks correctly without the tedium of figuring out the paths!</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c8772-147">Microsoft 사이트에 대한 링크에 ko-kr와 같은 로캘 코드를 포함하지 마세요.</span><span class="sxs-lookup"><span data-stu-id="c8772-147">Do not include locale codes, such as en-us, in your links to Microsoft sites.</span></span> <span data-ttu-id="c8772-148">하드 코딩된 로캘 코드는 지역화된 콘텐츠가 렌더링되지 못하게 합니다. 이는 다른 로캘의 사용자에게 좋지 않은 고객 환경이며 상당한 지역화 비용이 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-148">Hard-coded locale codes prevent localized content from rendering, which is a bad customer experience for users in other locales and incurs significant localization costs.</span></span> <span data-ttu-id="c8772-149">브라우저에서 URL을 복사하면 로캘 코드가 기본적으로 포함되므로 링크를 만들 때 수동으로 삭제해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-149">When you copy a URL from a browser, the locale code is included by default, so you need to manually delete in when you create your link.</span></span> <span data-ttu-id="c8772-150">예를 들어 다음을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-150">For example, use:</span></span>
>
> `[Microsoft](https://www.microsoft.com)`
>
> <span data-ttu-id="c8772-151">다음을 사용하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-151">Not:</span></span>
>
> `[Microsoft](https://www.microsoft.com/en-us/)`

### <a name="relative-links-to-files-in-the-same-doc-set"></a><span data-ttu-id="c8772-152">동일한 문서 집합에서 파일에 대한 상대 링크</span><span class="sxs-lookup"><span data-stu-id="c8772-152">Relative links to files in the same doc set</span></span>

<span data-ttu-id="c8772-153">상대 경로는 현재 파일을 기준으로 대상 파일에 대한 경로입니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-153">A relative path is the path to the target file relative to the current file.</span></span> <span data-ttu-id="c8772-154">OPS에서는 상대 경로를 사용하여 동일한 문서 집합 내의 다른 파일에 연결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-154">In OPS, you can use a relative path to link to another file within the same doc set.</span></span> <span data-ttu-id="c8772-155">상대 경로에 대한 구문은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-155">The syntax for a relative path is as follows:</span></span>

```markdown
[link text](../../folder/filename.md)
```

<span data-ttu-id="c8772-156">여기서 `../`는 계층 구조에서 한 수준 위를 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-156">Where `../` indicates one level above in the hierarchy.</span></span>

- <span data-ttu-id="c8772-157">상대 경로는 빌드 중에 .md 확장명 제거를 포함하여 확인됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-157">The relative path will be resolved during the build, including removal of the .md extension.</span></span>
- <span data-ttu-id="c8772-158">“../”를 사용하여 부모 폴더의 파일에 연결할 수 있지만, 해당 파일이 같은 문서 집합에 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-158">You can use "../" to link to a file in the parent folder, but that file has to be in the same doc set.</span></span> <span data-ttu-id="c8772-159">“../”를 사용하여 다른 문서 집합 폴더의 파일에 연결할 수는 없습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-159">You cannot use "../" to link to a file in another doc set folder.</span></span>
- <span data-ttu-id="c8772-160">OPS는 또한 “~”로 시작하는 특별한 양식의 상대 경로(예: ~/foo/bar.md)도 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-160">OPS also supports a special form of relative path that starts with "~" (for example, ~/foo/bar.md).</span></span> <span data-ttu-id="c8772-161">이 구문은 문서 집합의 루트 폴더를 기준으로 한 파일임을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-161">This syntax indicates a file relative to the root folder of a doc set.</span></span> <span data-ttu-id="c8772-162">이러한 종류의 경로도 빌드 중에 유효성이 검사되고 확인됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-162">This kind of path is also validated and resolved during the build.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c8772-163">상대 경로에 파일 확장명을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-163">Include the file extension in the relative path.</span></span> <span data-ttu-id="c8772-164">빌드는 상대 경로의 대상 파일이 있는지를 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-164">Build validates the existence of the target file of that relative path.</span></span> <span data-ttu-id="c8772-165">상대 경로에 파일 확장명이 포함되어 있지 않으면 빌드가 끊어진 링크 경고를 보고합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-165">If relative path does not include file extension, it is likely build will report a warning of broken link.</span></span> <span data-ttu-id="c8772-166">예를 들어 다음을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-166">For example, use:</span></span>
>
> `[link text](../../folder/filename.md)`
>
> <span data-ttu-id="c8772-167">다음을 사용하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-167">Not:</span></span>
>
> `[link text](../../folder/filename)`

### <a name="absolute-links-to-other-files-in-ops"></a><span data-ttu-id="c8772-168">OPS에서 다른 파일에 대한 절대 링크</span><span class="sxs-lookup"><span data-stu-id="c8772-168">Absolute links to other files in OPS</span></span>

```markdown
[Azure and Linux](/articles/virtual-machines/linux/overview)
```

<span data-ttu-id="c8772-169">파일 확장명(.md)을 포함하지 마세요.</span><span class="sxs-lookup"><span data-stu-id="c8772-169">Do not include the file extension (.md).</span></span> <span data-ttu-id="c8772-170">이것은 Azure “articles” 문서 집합 외부의 Linux 개요 파일에 연결됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-170">This links to the Linux overview file from outside the Azure "articles" doc set.</span></span>

### <a name="links-to-external-sites"></a><span data-ttu-id="c8772-171">외부 사이트로 연결</span><span class="sxs-lookup"><span data-stu-id="c8772-171">Links to external sites</span></span>

```markdown
[Microsoft](https://www.microsoft.com)
```

<span data-ttu-id="c8772-172">다른 웹 페이지로 URL 기반 연결(https://를 포함해야 함)입니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-172">URL-based link to another web page (must include https://).</span></span>

### <a name="bookmark-links"></a><span data-ttu-id="c8772-173">책갈피 링크</span><span class="sxs-lookup"><span data-stu-id="c8772-173">Bookmark links</span></span>

<span data-ttu-id="c8772-174">같은 리포지토리의 다른 파일 제목에 대한 책갈피 링크</span><span class="sxs-lookup"><span data-stu-id="c8772-174">Bookmark link to a heading in another file in the same repo:</span></span>

```markdown
[Managed Disks](../../linux/overview.md#managed-disks)
```

<span data-ttu-id="c8772-175">현재 파일의 제목에 대한 책갈피 링크</span><span class="sxs-lookup"><span data-stu-id="c8772-175">Bookmark link to a heading in the current file:</span></span>

```markdown
[Managed Disks](#managed-disks)
```

<span data-ttu-id="c8772-176">해시 태그 다음에 구두점이 제거되고 공백이 대시로 바뀐 제목의 단어를 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="c8772-176">Use a hash tag followed by the words of the heading with punctuation removed and spaces replaced with dashes.</span></span>

### <a name="explicit-anchor-links"></a><span data-ttu-id="c8772-177">명시적 앵커 링크</span><span class="sxs-lookup"><span data-stu-id="c8772-177">Explicit anchor links</span></span>

<span data-ttu-id="c8772-178">허브 및 방문 페이지를 제외하고는 `<a>` HTML 태그를 사용하는 명시적 앵커 링크가 **필요하거나 권장되지 않습니다.**</span><span class="sxs-lookup"><span data-stu-id="c8772-178">Explicit anchor links using the `<a>` HTML tag are **not required or recommended** except in hub and landing pages.</span></span> <span data-ttu-id="c8772-179">일반 Markdown 파일에 위에서 설명한 대로 책갈피를 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="c8772-179">Use bookmarks as described above in general Markdown files.</span></span> <span data-ttu-id="c8772-180">허브 및 방문 페이지의 경우 다음과 같이 앵커를 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="c8772-180">For hub and landing pages, use anchors as follows:</span></span>

<span data-ttu-id="c8772-181">`## <a id="AnchorText"> </a>Header text` 또는 `## <a name="AnchorText"> </a>Header text`</span><span class="sxs-lookup"><span data-stu-id="c8772-181">`## <a id="AnchorText"> </a>Header text` or `## <a name="AnchorText"> </a>Header text`</span></span>

<span data-ttu-id="c8772-182">명시적 앵커에 연결하려면 다음 구문을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-182">To link to explicit anchors, use the following syntax:</span></span>

```markdown
To go to a section on the same page:
[text](#AnchorText)

To go to a section on another page.
[text](FileName.md#AnchorText)
```

### <a name="xref-cross-reference-links"></a><span data-ttu-id="c8772-183">XREF(상호 참조) 링크</span><span class="sxs-lookup"><span data-stu-id="c8772-183">XREF (cross reference) links</span></span>

<span data-ttu-id="c8772-184">현재 문서 집합 또는 다른 문서 집합에서 자동 생성된 API 참조 페이지에 연결하려면 UID(고유한 ID)와 함께 XREF 링크를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-184">To link to auto-generated API references pages in the current doc set or other doc sets, use XREF links with the unique ID (UID).</span></span>

> [!NOTE]
> <span data-ttu-id="c8772-185">다른 문서 집합에서 API 참조 페이지를 참조하려면 `docfx.json` 파일에서 `xrefService` 구성을 추가해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-185">To reference API reference pages in other docsets, you need to add `xrefService` configuration in `docfx.json` file.</span></span>
> ```
> "build": {
>   ...
>   "xrefService": [ "https://xref.docs.microsoft.com/query?uid={uid}" ]
> }
> ```

<span data-ttu-id="c8772-186">UID는 정규화된 클래스 및 멤버 이름과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-186">The UID equates to the fully qualified class and member name.</span></span> <span data-ttu-id="c8772-187">UID 뒤에 \*를 추가하면 링크는 특정 API가 아닌 오버로드 페이지를 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-187">If you add a \* after the UID, the link then represents the overload page and not a specific API.</span></span> <span data-ttu-id="c8772-188">예를 들어 `List<T>.BinarySearch*`를 사용하여 `List<T>.BinarySearch(T, IComparer<T>)`와 같은 특정 과부하로 연결하는 대신 BinarySearch 메서드 페이지에 연결합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-188">For example, use `List<T>.BinarySearch*` to link to the BinarySearch Method page instead of linking to a specific overload such as `List<T>.BinarySearch(T, IComparer<T>)`.</span></span>

<span data-ttu-id="c8772-189">다음 구문 중 하나를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-189">You can use one of the following syntaxes:</span></span>

- <span data-ttu-id="c8772-190">자동 연결: `<xref:UID> or <xref:UID?displayProperty=nameWithType>`</span><span class="sxs-lookup"><span data-stu-id="c8772-190">Auto-link: `<xref:UID> or <xref:UID?displayProperty=nameWithType>`</span></span>

  <span data-ttu-id="c8772-191">선택적 `displayProperty` 쿼리 매개 변수는 정규화된 링크 텍스트를 생성합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-191">The optional `displayProperty` query parameter produces a fully qualified link text.</span></span> <span data-ttu-id="c8772-192">기본적으로 링크 텍스트는 멤버 또는 형식 이름만 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-192">By default, link text shows only the member or type name.</span></span>

- <span data-ttu-id="c8772-193">Markdown 링크: `[link text](xref:UID)`</span><span class="sxs-lookup"><span data-stu-id="c8772-193">Markdown link: `[link text](xref:UID)`</span></span>
  
  <span data-ttu-id="c8772-194">표시되는 링크 텍스트를 사용자 지정하려면 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-194">Use when you want to customize the link text displayed.</span></span>

<span data-ttu-id="c8772-195">예제:</span><span class="sxs-lookup"><span data-stu-id="c8772-195">Examples:</span></span>

- <span data-ttu-id="c8772-196">`<xref:System.String>`은 “String”으로 렌더링됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-196">`<xref:System.String>` renders as "String".</span></span>
- <span data-ttu-id="c8772-197">`<xref:System.String?displayProperty=nameWithType>`은 “System.String”으로 렌더링됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-197">`<xref:System.String?displayProperty=nameWithType>` renders as "System.String".</span></span>
- <span data-ttu-id="c8772-198">`[String class](xref:System.String)`는 “String class”로 렌더링됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-198">`[String class](xref:System.String)` renders as "String class".</span></span>

<span data-ttu-id="c8772-199">지금은 UID를 쉽게 찾는 방법이 없습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-199">Right now, there is no easy way to find the UIDs.</span></span> <span data-ttu-id="c8772-200"><!-- ? -->API의 UID를 찾는 가장 좋은 방법은 연결하려는 API 페이지의 소스를 보고 ms.assetid 값을 찾는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-200"><!-- ? -->The best way to find the UID for an API is to view the source for the API page you want to link to and find the ms.assetid value.</span></span> <span data-ttu-id="c8772-201">개별 오버로드 값은 소스에 표시되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-201">Individual overload values are not shown in the source.</span></span> <span data-ttu-id="c8772-202">Microsoft는 시스템 개선을 위해 노력하고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-202">We're working on having a better system in the future.</span></span>

<span data-ttu-id="c8772-203">UID에 특수 문자 \`, \# 또는 \*이 포함되는 경우 UID 값을 `%60`, `%23` 및 `%2A`로 각각 HTML 인코딩해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-203">When the UID contains the special characters \`, \#, or \*, the UID value needs to be HTML encoded as `%60`, `%23`, and `%2A`, respectively.</span></span> <span data-ttu-id="c8772-204">때때로 괄호 인코딩을 보게 되겠지만 이는 필요하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-204">You'll sometimes see parentheses encoded but it's not a requirement.</span></span>

<span data-ttu-id="c8772-205">예제:</span><span class="sxs-lookup"><span data-stu-id="c8772-205">Examples:</span></span>

- <span data-ttu-id="c8772-206">System.Threading.Tasks.Task\`1은 `System.Threading.Tasks.Task%601`이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-206">System.Threading.Tasks.Task\`1 becomes `System.Threading.Tasks.Task%601`</span></span>
- <span data-ttu-id="c8772-207">System.Exception.\#ctor은 `System.Exception.%23ctor`이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-207">System.Exception.\#ctor becomes `System.Exception.%23ctor`</span></span>
- <span data-ttu-id="c8772-208">System.Lazy\`1.\#ctor(System.Threading.LazyThreadSafetyMode)은 `System.Lazy%601.%23ctor%28System.Threading.LazyThreadSafetyMode%29`가 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-208">System.Lazy\`1.\#ctor(System.Threading.LazyThreadSafetyMode) becomes  `System.Lazy%601.%23ctor%28System.Threading.LazyThreadSafetyMode%29`</span></span>

<!-- leave out of Contributor Guide for now
Using XREF may require some configuration. For more information, see XREF Service.
-->

## <a name="lists-numbered-bulleted-checklist"></a><span data-ttu-id="c8772-209">목록(번호 매김, 글머리 기호, 검사 목록)</span><span class="sxs-lookup"><span data-stu-id="c8772-209">Lists (Numbered, Bulleted, Checklist)</span></span>

### <a name="numbered-list"></a><span data-ttu-id="c8772-210">번호 매기기 목록</span><span class="sxs-lookup"><span data-stu-id="c8772-210">Numbered list</span></span>

<span data-ttu-id="c8772-211">번호 매기기 목록을 만들려면, 모두 1을 사용할 수 있으며 이것은 게시할 때 순차 목록으로 렌더링됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-211">To create a numbered list, you can use all 1s, which are rendered as a sequential list when published.</span></span> <span data-ttu-id="c8772-212">소스 가독성을 높이기 위해 목록을 증가시킬 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-212">For increased source readability, you can increment your lists.</span></span>

<span data-ttu-id="c8772-213">중첩 목록을 포함하여 목록에 문자를 사용하지 마세요.</span><span class="sxs-lookup"><span data-stu-id="c8772-213">Do not use letters in lists, including nested lists.</span></span> <span data-ttu-id="c8772-214">OPS를 통해 게시할 때 올바르게 렌더링되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-214">They do not render correctly when published via OPS.</span></span> <span data-ttu-id="c8772-215">숫자를 사용하여 중첩된 목록은 게시될 때 소문자로 렌더링됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-215">Nested lists using numbers will render as lowercase letters when published.</span></span> <span data-ttu-id="c8772-216">예:</span><span class="sxs-lookup"><span data-stu-id="c8772-216">For example:</span></span>

```markdown
1. This is
1. a parent numbered list
   1. and this is
   1. a nested numbered list
1. (fin)
```

<span data-ttu-id="c8772-217">이것은 다음과 같이 렌더링됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-217">This renders as follows:</span></span>

1. <span data-ttu-id="c8772-218">This is</span><span class="sxs-lookup"><span data-stu-id="c8772-218">This is</span></span>
1. <span data-ttu-id="c8772-219">a parent numbered list</span><span class="sxs-lookup"><span data-stu-id="c8772-219">a parent numbered list</span></span>
   1. <span data-ttu-id="c8772-220">and this is</span><span class="sxs-lookup"><span data-stu-id="c8772-220">and this is</span></span>
   1. <span data-ttu-id="c8772-221">a nested numbered list</span><span class="sxs-lookup"><span data-stu-id="c8772-221">a nested numbered list</span></span>
1. <span data-ttu-id="c8772-222">(fin)</span><span class="sxs-lookup"><span data-stu-id="c8772-222">(fin)</span></span>

### <a name="bulleted-list"></a><span data-ttu-id="c8772-223">글머리 기호 목록</span><span class="sxs-lookup"><span data-stu-id="c8772-223">Bulleted list</span></span>

<span data-ttu-id="c8772-224">글머리 기호 목록을 만들려면 각 줄의 시작 위치에 `-`와 공백을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-224">To create a bulleted list, use `-` followed by a space at the beginning of each line:</span></span>

```markdown
- This is
- a parent bulleted list
  - and this is
  - a nested bulleted list
- All done!
```

<span data-ttu-id="c8772-225">이것은 다음과 같이 렌더링됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-225">This renders as follows:</span></span>

- <span data-ttu-id="c8772-226">This is</span><span class="sxs-lookup"><span data-stu-id="c8772-226">This is</span></span>
- <span data-ttu-id="c8772-227">a parent bulleted list</span><span class="sxs-lookup"><span data-stu-id="c8772-227">a parent bulleted list</span></span>
  - <span data-ttu-id="c8772-228">and this is</span><span class="sxs-lookup"><span data-stu-id="c8772-228">and this is</span></span>
  - <span data-ttu-id="c8772-229">a nested bulleted list</span><span class="sxs-lookup"><span data-stu-id="c8772-229">a nested bulleted list</span></span>
- <span data-ttu-id="c8772-230">All done!</span><span class="sxs-lookup"><span data-stu-id="c8772-230">All done!</span></span>

### <a name="checklist"></a><span data-ttu-id="c8772-231">검사 목록</span><span class="sxs-lookup"><span data-stu-id="c8772-231">Checklist</span></span>

<span data-ttu-id="c8772-232">검사 목록은 사용자 지정 Markdown 확장을 통해 docs.microsoft.com에서만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-232">Checklists are available for use on docs.microsoft.com (only) via a custom Markdown extension:</span></span>

```markdown
> [!div class="checklist"]
> * List item 1
> * List item 2
> * List item 3
```

<span data-ttu-id="c8772-233">이 예제는 다음과 같이 docs.microsoft.com에서 렌더링됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-233">This example renders on docs.microsoft.com like this:</span></span>

> [!div class="checklist"]
> * <span data-ttu-id="c8772-234">목록 항목 1</span><span class="sxs-lookup"><span data-stu-id="c8772-234">List item 1</span></span>
> * <span data-ttu-id="c8772-235">목록 항목 2</span><span class="sxs-lookup"><span data-stu-id="c8772-235">List item 2</span></span>
> * <span data-ttu-id="c8772-236">목록 항목 3</span><span class="sxs-lookup"><span data-stu-id="c8772-236">List item 3</span></span>

<span data-ttu-id="c8772-237">문서의 처음이나 끝에 있는 검사 목록을 사용하여 “배울 내용” 또는 “배운 내용” 콘텐츠를 요약합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-237">Use checklits at the beginning or end of an article to summarize "What will you learn" or "What have you learned" content.</span></span> <span data-ttu-id="c8772-238">문서 전체에 임의의 검사 목록을 추가하지 마세요.</span><span class="sxs-lookup"><span data-stu-id="c8772-238">Do not add random checklists throughout your articles.</span></span>
<!-- is this guidance still accurate? -->

## <a name="next-step-action"></a><span data-ttu-id="c8772-239">다음 단계 작업</span><span class="sxs-lookup"><span data-stu-id="c8772-239">Next step action</span></span>

<span data-ttu-id="c8772-240">사용자 지정 확장 프로그램을 사용하여 docs.microsoft.com의 페이지에만 다음 단계 작업 단추를 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-240">You can use a custom extension to add a next step action button to pages on docs.microsoft.com (only).</span></span>

<span data-ttu-id="c8772-241">구문은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-241">The syntax is as follows:</span></span>

```markdown
> [!div class="nextstepaction"]
> [button text](link to topic)
```

<span data-ttu-id="c8772-242">예:</span><span class="sxs-lookup"><span data-stu-id="c8772-242">For example:</span></span>

```markdown
> [!div class="nextstepaction"]
> [Learn about basic style](style-quick-start.md)
```

<span data-ttu-id="c8772-243">이것은 다음과 같이 렌더링됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-243">This renders as follows:</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="c8772-244">기본 스타일에 대한 자세한 정보</span><span class="sxs-lookup"><span data-stu-id="c8772-244">Learn about basic style</span></span>](style-quick-start.md)

<span data-ttu-id="c8772-245">다른 웹 페이지에 대한 Markdown 링크를 포함하여 다음 단계 작업에서 지원되는 링크를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-245">You can use any supported link in a next step action, including a Markdown link to another web page.</span></span> <span data-ttu-id="c8772-246">대부분의 경우 다음 작업 링크는 동일한 문서 집합에 있는 다른 파일에 대한 상대 링크입니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-246">In most cases, the next action link will be a relative link to another file in the same doc set.</span></span>

## <a name="section-definition"></a><span data-ttu-id="c8772-247">섹션 정의</span><span class="sxs-lookup"><span data-stu-id="c8772-247">Section definition</span></span>

<span data-ttu-id="c8772-248"><!-- more info about this would be helpful! --> 섹션을 정의해야 할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-248"><!-- more info about this would be helpful! --> You might need to define a section.</span></span> <span data-ttu-id="c8772-249">이 구문은 대개 코드 테이블에 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-249">This syntax is mostly used for code tables.</span></span>
<span data-ttu-id="c8772-250">다음 예제를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c8772-250">See the following example:</span></span>

````
> [!div class="tabbedCodeSnippets" data-resources="OutlookServices.Calendar"]
> ```cs
> <cs code text>
> ```
> ```javascript
> <js code text>
> ```
````

<span data-ttu-id="c8772-251">앞의 blockquote Markdown 텍스트는 다음과 같이 렌더링됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-251">The preceding blockquote Markdown text will be rendered as:</span></span>
> [!div class="tabbedCodeSnippets" data-resources="OutlookServices.Calendar"]
> ```cs
> <cs code text>
> ```
> ```javascript
> <js code text>
> ```

## <a name="selectors"></a><span data-ttu-id="c8772-252">선택기</span><span class="sxs-lookup"><span data-stu-id="c8772-252">Selectors</span></span>

<span data-ttu-id="c8772-253"><!-- could be more clear! --> 같은 문서의 다른 페이지에 연결하려면 선택기를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-253"><!-- could be more clear! --> You can use a selector when you want to connect different pages for the same article.</span></span> <span data-ttu-id="c8772-254">그러면 독자는 해당 페이지 간에 전환할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-254">Readers can then switch between those pages.</span></span>

> [!NOTE]
> <span data-ttu-id="c8772-255">이 확장은 docs.microsoft.com과 MSDN에서 서로 다르게 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-255">This extension works differently between docs.microsoft.com and MSDN.</span></span> <!-- should we keep info about MSDN? If so say how they differ?-->

### <a name="single-selector"></a><span data-ttu-id="c8772-256">단일 선택기</span><span class="sxs-lookup"><span data-stu-id="c8772-256">Single selector</span></span>

```
> [!div class="op_single_selector"]
> - [Universal Windows](how-to-write-use-markdown.md)
> - [Windows Phone](how-to-write-use-markdown.md)
> - [iOS](how-to-write-use-markdown.md)
> - [Android](how-to-write-use-markdown.md)
> - [Kindle](how-to-write-use-markdown.md)
> - [Baidu](how-to-write-use-markdown.md)
> - [Xamarin.iOS](how-to-write-use-markdown.md)
> - [Xamarin.Android](how-to-write-use-markdown.md)
```

<span data-ttu-id="c8772-257">다음과 같이 렌더링됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-257">... will be rendered like this:</span></span>

> [!div class="op_single_selector"]
> - [유니버설 Windows](how-to-write-use-markdown.md)
> - [Windows Phone](how-to-write-use-markdown.md)
> - [iOS](how-to-write-use-markdown.md)
> - [Android](how-to-write-use-markdown.md)
> - [Kindle](how-to-write-use-markdown.md)
> - [Baidu](how-to-write-use-markdown.md)
> - [Xamarin.iOS](how-to-write-use-markdown.md)
> - [Xamarin.Android](how-to-write-use-markdown.md)

### <a name="multi-selector"></a><span data-ttu-id="c8772-266">다중 선택기</span><span class="sxs-lookup"><span data-stu-id="c8772-266">Multi-selector</span></span>

```
> [!div class="op_multi_selector" title1="Platform" title2="Backend"]
> - [(iOS | .NET)](how-to-write-workflows-major.md)
> - [(iOS | JavaScript)](how-to-write-workflows-major.md)
> - [(Windows universal C# | .NET)](how-to-write-workflows-major.md)
> - [(Windows universal C# | Javascript)](how-to-write-workflows-major.md)
> - [(Windows Phone | .NET)](how-to-write-workflows-major.md)
> - [(Windows Phone | Javascript)](how-to-write-workflows-major.md)
> - [(Android | .NET)](how-to-write-workflows-major.md)
> - [(Android | Javascript)](how-to-write-workflows-major.md)
> - [(Xamarin iOS | Javascript)](how-to-write-workflows-major.md)
> - [(Xamarin Android | Javascript)](how-to-write-workflows-major.md)
```

<span data-ttu-id="c8772-267">다음과 같이 렌더링됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-267">... will be rendered like this:</span></span>

> [!div class="op_multi_selector" title1="Platform" title2="Backend"]
> - [(iOS | .NET)](how-to-write-workflows-major.md)
> - [(iOS | JavaScript)](how-to-write-workflows-major.md)
> - [(Windows 유니버설 C# | .NET)](how-to-write-workflows-major.md)
> - [(Windows 유니버설 C# | Javascript)](how-to-write-workflows-major.md)
> - [(Windows Phone | .NET)](how-to-write-workflows-major.md)
> - [(Windows Phone | Javascript)](how-to-write-workflows-major.md)
> - [(Android | .NET)](how-to-write-workflows-major.md)
> - [(Android | Javascript)](how-to-write-workflows-major.md)
> - [(Xamarin iOS | Javascript)](how-to-write-workflows-major.md)
> - [(Xamarin Android | Javascript)](how-to-write-workflows-major.md)

<!-- uncomment and link when Cory's topic is live
## Tabbed content

Tabs are a Markdown extension for docs.microsoft.com that allow us to present different versions of content, such as procedural steps to accomplish the same task on different platforms, in a tabbed format.

Because the syntax and requirements for tabbed content are fairly complex, they are documented separately in Tabbed Content.
-->

## <a name="tables"></a><span data-ttu-id="c8772-278">보세요.</span><span class="sxs-lookup"><span data-stu-id="c8772-278">Tables</span></span>

<span data-ttu-id="c8772-279">Markdown에서 테이블을 만드는 가장 간단한 방법은 파이프 및 줄을 사용하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-279">The simplest way to create a table in Markdown is to use pipes and lines.</span></span> <span data-ttu-id="c8772-280">헤더가 있는 표준 테이블을 만들려면 첫 번째 선을 파선으로 그립니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-280">To create a standard table with a header, follow the first line with dashed line:</span></span>

```markdown
|This is   |a simple   |table header|
|----------|-----------|------------|
|table     |data       |here        |
|it doesn't|actually   |have to line up nicely!|
```

<span data-ttu-id="c8772-281">이것은 다음과 같이 렌더링됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-281">This renders as follows:</span></span>

|<span data-ttu-id="c8772-282">This is</span><span class="sxs-lookup"><span data-stu-id="c8772-282">This is</span></span>   |<span data-ttu-id="c8772-283">a simple</span><span class="sxs-lookup"><span data-stu-id="c8772-283">a simple</span></span>   |<span data-ttu-id="c8772-284">table header</span><span class="sxs-lookup"><span data-stu-id="c8772-284">table header</span></span>|
|----------|-----------|------------|
|<span data-ttu-id="c8772-285">table</span><span class="sxs-lookup"><span data-stu-id="c8772-285">table</span></span>     |<span data-ttu-id="c8772-286">data</span><span class="sxs-lookup"><span data-stu-id="c8772-286">data</span></span>       |<span data-ttu-id="c8772-287">here</span><span class="sxs-lookup"><span data-stu-id="c8772-287">here</span></span>        |
|<span data-ttu-id="c8772-288">it doesn't</span><span class="sxs-lookup"><span data-stu-id="c8772-288">it doesn't</span></span>|<span data-ttu-id="c8772-289">actually</span><span class="sxs-lookup"><span data-stu-id="c8772-289">actually</span></span>   |<span data-ttu-id="c8772-290">have to line up nicely!</span><span class="sxs-lookup"><span data-stu-id="c8772-290">have to line up nicely!</span></span>||

<span data-ttu-id="c8772-291">헤더가 없는 테이블을 만들 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-291">You can also create a table without a header.</span></span> <span data-ttu-id="c8772-292">예를 들어 다중 열 목록을 만들려면:</span><span class="sxs-lookup"><span data-stu-id="c8772-292">For example, to create a multiple-column list:</span></span>

```markdown
|   |   |
| - | - |
| This | table |
| has no | header |
```

<span data-ttu-id="c8772-293">다음과 같이 렌더링됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-293">This renders like this:</span></span>

|   |   |
| - | - |
| <span data-ttu-id="c8772-294">This</span><span class="sxs-lookup"><span data-stu-id="c8772-294">This</span></span> | <span data-ttu-id="c8772-295">table</span><span class="sxs-lookup"><span data-stu-id="c8772-295">table</span></span> |
| <span data-ttu-id="c8772-296">has no</span><span class="sxs-lookup"><span data-stu-id="c8772-296">has no</span></span> | <span data-ttu-id="c8772-297">header</span><span class="sxs-lookup"><span data-stu-id="c8772-297">header</span></span> |

<span data-ttu-id="c8772-298">콜론을 사용하여 열을 정렬할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-298">You can align the columns by using colons:</span></span>

```markdown
|                  |
|------------------|
|    right aligned:|
|:left aligned     |
|:centered        :|
```

<span data-ttu-id="c8772-299">다음과 같이 렌더링됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-299">Renders as follows:</span></span>

|                  |
|------------------|
|    <span data-ttu-id="c8772-300">right aligned:</span><span class="sxs-lookup"><span data-stu-id="c8772-300">right aligned:</span></span>|
|<span data-ttu-id="c8772-301">:left aligned</span><span class="sxs-lookup"><span data-stu-id="c8772-301">:left aligned</span></span>     |
|<span data-ttu-id="c8772-302">:centered        :</span><span class="sxs-lookup"><span data-stu-id="c8772-302">:centered        :</span></span>|

> [!TIP]
> VS Code용 Docs Authoring Extension을 사용하면 기본 Markdown 테이블을 쉽게 추가할 수 있습니다!
>
> [온라인 테이블 생성기](http://www.tablesgenerator.com/markdown_tables)를 사용할 수도 있습니다.

### <a name="mx-tdbreakall"></a><span data-ttu-id="c8772-305">mx-tdBreakAll</span><span class="sxs-lookup"><span data-stu-id="c8772-305">mx-tdBreakAll</span></span>

> [!IMPORTANT]
> 이것은 docs.microsoft.com 사이트에서만 작동합니다.

<span data-ttu-id="c8772-307">Markdown에서 테이블을 만드는 경우 테이블이 오른쪽 탐색으로 확장되어 읽을 수 없게 될 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-307">If you create a table in Markdown, the table might expand to the right navigation and become unreadable.</span></span> <span data-ttu-id="c8772-308">필요한 경우 문서 렌더링에서 테이블을 나눌 수 있도록 허용하여 이 문제를 해결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-308">You can solve that by allowing Docs rendering to break the table when needed.</span></span> <span data-ttu-id="c8772-309">`[!div class="mx-tdBreakAll"]` 사용자 지정 클래스로 테이블을 래핑하기만 하면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-309">Just wrap up the table with the custom class `[!div class="mx-tdBreakAll"]`.</span></span>

<span data-ttu-id="c8772-310">다음은 클래스 이름이 `mx-tdBreakAll`인 `div`로 래핑될 행이 세 개인 테이블의 Markdown 샘플입니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-310">Here is a Markdown sample of a table with three rows that will be wrapped by a `div` with the class name `mx-tdBreakAll`.</span></span>

```markdown
> [!div class="mx-tdBreakAll"]
> |Name|Syntax|Mandatory for silent installation?|Description|
> |-------------|----------|---------|---------|
> |Quiet|/quiet|Yes|Runs the installer, displaying no UI and no prompts.|
> |NoRestart|/norestart|No|Suppresses any attempts to restart. By default, the UI will prompt before restart.|
> |Help|/help|No|Provides help and quick reference. Displays the correct use of the setup command, including a list of all options and behaviors.|
```

<span data-ttu-id="c8772-311">다음과 같이 렌더링됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-311">It will be rendered like this:</span></span>

> [!div class="mx-tdBreakAll"]
> |<span data-ttu-id="c8772-312">이름</span><span class="sxs-lookup"><span data-stu-id="c8772-312">Name</span></span>|<span data-ttu-id="c8772-313">구문</span><span class="sxs-lookup"><span data-stu-id="c8772-313">Syntax</span></span>|<span data-ttu-id="c8772-314">자동 설치에 필수인지 여부</span><span class="sxs-lookup"><span data-stu-id="c8772-314">Mandatory for silent installation?</span></span>|<span data-ttu-id="c8772-315">설명</span><span class="sxs-lookup"><span data-stu-id="c8772-315">Description</span></span>|
> |-------------|----------|---------|---------|
> |<span data-ttu-id="c8772-316">Quiet</span><span class="sxs-lookup"><span data-stu-id="c8772-316">Quiet</span></span>|<span data-ttu-id="c8772-317">/quiet</span><span class="sxs-lookup"><span data-stu-id="c8772-317">/quiet</span></span>|<span data-ttu-id="c8772-318">예</span><span class="sxs-lookup"><span data-stu-id="c8772-318">Yes</span></span>|<span data-ttu-id="c8772-319">UI와 프롬프트를 표시하지 않고 설치 관리자를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-319">Runs the installer, displaying no UI and no prompts.</span></span>|
> |<span data-ttu-id="c8772-320">NoRestart</span><span class="sxs-lookup"><span data-stu-id="c8772-320">NoRestart</span></span>|<span data-ttu-id="c8772-321">/norestart</span><span class="sxs-lookup"><span data-stu-id="c8772-321">/norestart</span></span>|<span data-ttu-id="c8772-322">아니요</span><span class="sxs-lookup"><span data-stu-id="c8772-322">No</span></span>|<span data-ttu-id="c8772-323">다시 시작하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-323">Suppresses any attempts to restart.</span></span> <span data-ttu-id="c8772-324">기본적으로 다시 시작하기 전에 UI가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-324">By default, the UI will prompt before restart.</span></span>|
> |<span data-ttu-id="c8772-325">Help</span><span class="sxs-lookup"><span data-stu-id="c8772-325">Help</span></span>|<span data-ttu-id="c8772-326">/help</span><span class="sxs-lookup"><span data-stu-id="c8772-326">/help</span></span>|<span data-ttu-id="c8772-327">아니요</span><span class="sxs-lookup"><span data-stu-id="c8772-327">No</span></span>|<span data-ttu-id="c8772-328">도움말 및 빠른 참조를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-328">Provides help and quick reference.</span></span> <span data-ttu-id="c8772-329">모든 옵션 및 동작 목록을 비롯한 설정 명령의 올바른 사용법을 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-329">Displays the correct use of the setup command, including a list of all options and behaviors.</span></span>|

### <a name="mx-tdcol2breakall"></a><span data-ttu-id="c8772-330">mx-tdCol2BreakAll</span><span class="sxs-lookup"><span data-stu-id="c8772-330">mx-tdCol2BreakAll</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c8772-331">이것은 docs.microsoft.com 사이트에서만 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-331">This only works on the docs.microsoft.com site.</span></span>

<span data-ttu-id="c8772-332">때때로 테이블의 두 번째 열에 매우 긴 단어가 표시될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-332">From time to time, you might have very long words in the second column of a table.</span></span> <span data-ttu-id="c8772-333">이것을 깔끔하게 분리하려면 앞서 보았듯이 `div` 래퍼 구문을 사용하여 `mx-tdCol2BreakAll` 클래스를 적용하면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-333">To ensure they are broken apart nicely, you can apply the class `mx-tdCol2BreakAll` by using the `div` wrapper syntax as shown earlier.</span></span>

### <a name="html-tables"></a><span data-ttu-id="c8772-334">HTML 테이블</span><span class="sxs-lookup"><span data-stu-id="c8772-334">HTML Tables</span></span>

<span data-ttu-id="c8772-335">HTML 테이블은 docs.microsoft.com에 사용하지 않는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-335">HTML tables are not recommended for docs.microsoft.com.</span></span> <span data-ttu-id="c8772-336">소스에서 사람이 읽을 수 없으며 이것이 Markdown의 핵심 원칙입니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-336">They are not human readable in the source - which is a key principle of Markdown.</span></span>

<!--If you use HTML tables and your Markdown is not being rendered between the two tables, you need to add a closing `br` tag after the closing `table` tag.

![break HTML tables](media/break-tables.png)
-->

## <a name="videos"></a><span data-ttu-id="c8772-337">비디오</span><span class="sxs-lookup"><span data-stu-id="c8772-337">Videos</span></span>

### <a name="embedding-videos-into-a-markdown-page"></a><span data-ttu-id="c8772-338">Markdown 페이지에 비디오 포함</span><span class="sxs-lookup"><span data-stu-id="c8772-338">Embedding videos into a Markdown page</span></span>

<span data-ttu-id="c8772-339">현재, OPS는 다음 3가지 위치 중 하나에 게시된 비디오를 지원할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-339">Currently, OPS can support videos published to one of three locations:</span></span>

- <span data-ttu-id="c8772-340">YouTube</span><span class="sxs-lookup"><span data-stu-id="c8772-340">YouTube</span></span>
- <span data-ttu-id="c8772-341">Channel9</span><span class="sxs-lookup"><span data-stu-id="c8772-341">Channel 9</span></span>
- <span data-ttu-id="c8772-342">Microsoft 고유 'One Player' 시스템</span><span class="sxs-lookup"><span data-stu-id="c8772-342">Microsoft's own 'One Player' system</span></span>

<span data-ttu-id="c8772-343">다음 구문으로 비디오를 포함할 수 있으며, 포함하면 OPS에서 렌더링합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-343">You can embed a video with the following syntax, and OPS will render it.</span></span>

```markdown
> [!VIDEO <embedded_video_link>]
```

<span data-ttu-id="c8772-344">예제:</span><span class="sxs-lookup"><span data-stu-id="c8772-344">Example:</span></span>

```markdown
> [!VIDEO https://channel9.msdn.com/Series/Youve-Got-Key-Values-A-Redis-Jump-Start/03/player]

> [!VIDEO https://www.youtube.com/embed/iAtwVM-Z7rY]

> [!VIDEO https://www.microsoft.com/en-us/videoplayer/embed/RE1XVQS]
```

<span data-ttu-id="c8772-345">다음과 같이 렌더링됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-345">... will be rendered as:</span></span>

```html
<iframe src="https://channel9.msdn.com/Series/Youve-Got-Key-Values-A-Redis-Jump-Start/03/player" width="640" height="320" allowFullScreen="true" frameBorder="0"></iframe>

<iframe src="https://www.youtube-nocookie.com/embed/iAtwVM-Z7rY" width="640" height="320" allowFullScreen="true" frameBorder="0"></iframe>
<iframe src="https://www.microsoft.com/en-us/videoplayer/embed/RE1XVQS" width="640" height="320" allowFullScreen="true" frameBorder="0"></iframe>
```

<span data-ttu-id="c8772-346">그리고 게시된 페이지에 다음과 같이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-346">And it will be displayed like this on published pages:</span></span>

> [!VIDEO https://channel9.msdn.com/Series/Youve-Got-Key-Values-A-Redis-Jump-Start/03/player]

> [!VIDEO https://www.youtube.com/embed/iAtwVM-Z7rY]

> [!VIDEO https://www.microsoft.com/en-us/videoplayer/embed/RE1XVQS]

> [!IMPORTANT]
> <span data-ttu-id="c8772-347">CH9 비디오 URL은 `https`로 시작하고 `/player`로 끝나야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-347">The CH9 video URL should start with `https` and end with `/player`.</span></span> <span data-ttu-id="c8772-348">그렇지 않으면 비디오만이 아니라 전체 페이지를 포함하게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-348">Otherwise, it will embed the whole page instead of the video only.</span></span>

### <a name="uploading-new-videos"></a><span data-ttu-id="c8772-349">새 비디오 업로딩</span><span class="sxs-lookup"><span data-stu-id="c8772-349">Uploading new videos</span></span>

<span data-ttu-id="c8772-350">모든 새 비디오는 다음 프로세스에 따라 업로드해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-350">Any new videos should be uploaded using the following process:</span></span>

1. <span data-ttu-id="c8772-351">IDWEB에서 **docs_video_users** 그룹에 조인합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-351">Join the **docs_video_users** group on IDWEB.</span></span>
1. <span data-ttu-id="c8772-352">https://aka.ms/VideoUploadRequest로 이동하고 비디오에 대한 세부 사항을 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-352">Go to https://aka.ms/VideoUploadRequest and fill in the details for your video.</span></span> <span data-ttu-id="c8772-353">다음이 필요합니다(이러한 항목은 공개되지 않음).</span><span class="sxs-lookup"><span data-stu-id="c8772-353">You will need (note that none of these items will be visible to the public):</span></span>
    1. <span data-ttu-id="c8772-354">비디오의 제목</span><span class="sxs-lookup"><span data-stu-id="c8772-354">A title for your video.</span></span>
    1. <span data-ttu-id="c8772-355">비디오가 관련된 제품/서비스 목록</span><span class="sxs-lookup"><span data-stu-id="c8772-355">A list of products/services that your video is related to.</span></span>
    1. <span data-ttu-id="c8772-356">비디오가 호스트되는 대상 페이지 또는 (아직 페이지가 없는 경우) 문서 집합</span><span class="sxs-lookup"><span data-stu-id="c8772-356">The target page or (if you don’t have the page yet) doc set that your video will be hosted on.</span></span>
    1. <span data-ttu-id="c8772-357">비디오에 대한 MP4 파일 링크(파일을 배치할 위치가 없으면 임시로 여기에 배치할 수 있음: `\\scratch2\scratch\apex`).</span><span class="sxs-lookup"><span data-stu-id="c8772-357">A link to the MP4 file for your video (if you don’t have a location to put the file, you can put it here temporarily:   `\\scratch2\scratch\apex`).</span></span> <span data-ttu-id="c8772-358">MP4 파일은 720p 이상이어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-358">MP4 files should be 720p or higher.</span></span>
    1. <span data-ttu-id="c8772-359">비디오 설명</span><span class="sxs-lookup"><span data-stu-id="c8772-359">A description of the video.</span></span>
1. <span data-ttu-id="c8772-360">항목을 제출(저장)합니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-360">Submit (save) that item.</span></span>
1. <span data-ttu-id="c8772-361">2 영업일 이내에 비디오가 업로드됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-361">Within two business days, the video will get uploaded.</span></span> <span data-ttu-id="c8772-362">포함에 필요한 링크가 작업 항목에 배치되고 확인되어 *전달됩니다*.</span><span class="sxs-lookup"><span data-stu-id="c8772-362">The link you need for embedding will be placed into the work item, and it will be resolved *back to you*.</span></span>
1. <span data-ttu-id="c8772-363">비디오 링크를 얻었으면 작업 항목을 닫습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-363">Once you have grabbed the video link, close the work item.</span></span>
1. <span data-ttu-id="c8772-364">다음 구문을 사용하여 비디오 링크를 게시물에 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8772-364">The video link can then be added to your post, using this syntax:</span></span>

   ```markdown
   > [!VIDEO https://www.microsoft.com/en-us/videoplayer/embed/RE1XVQS]
   ```