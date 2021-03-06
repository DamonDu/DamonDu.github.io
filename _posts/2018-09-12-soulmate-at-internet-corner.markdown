---
layout:     post
title:      "互联网角落的「Soulmate」"
subtitle:   "由 Soul 引发的一些思考"
date:       2018-09-12 07:00:00
author:     "Damon To"
header-style: text
catalog:    true
tags:
    - 产品
---

> 2018.12.12 更新：这篇文章逻辑和内容有硬伤，基本上只能看作一篇用户体验报告。缺乏参考性，仅供娱乐。

> 两个月前，我开始了自己的第一段实习，所在部门的主体业务是依附于手机 QQ 上的一个基于 LBS 的陌生人社交入口。虽然做的是后台开发，但是出于对陌生人社交这个场景的好奇，两个月以来也从产品和业务的角度了解到不少这个领域的现状。同时，之前和产品同事聊天时聊到了 Soul 这款陌生人社交 App，产生了不少的思考。这篇文章，尝试着从产品角度讲讲 Soul，也谈谈陌生人社交的现状和未来。

### Soul 与「心灵社交」

Soul 是一款主打**性格测试+算法推荐**的陌生人交友 APP，其主体功能——「心灵社交」的逻辑也足够简单：首先，用户首次进入时进行一次简单的”灵魂测试“；接着，依据测试结果，每个用户会落在不同的”星球“上；最后，当用户点击”Matching“进行系统匹配时，系统结合用户所在“星球”和其他性格特征来匹配“合拍度”高的其他用户。通过将 ”用户调研→生成用户画像→算法推荐“ 的流程进行了形象化地封装，再加上适度的引导，Soul 很大程度地抹除了用户对流程的天然反感，也契合产品自身的调性。

![](/img/in-post/2018-09-12-soulmate-at-internet-corner/soul_use_logic.png)

<center>    
	<div style="color:orange; border-bottom: 1px solid #d9d9d9;display: inline-block;     color: #999;padding: 1px;">一次「心灵社交」的简要流程</div> 
</center>

除了产品主体逻辑，Soul 还有一个重要的分支功能——**「广场」**，这是一个基于 UGC 的 Feed 流。用户可以在「广场」发布自己的「瞬间」，发布的「瞬间」将会被其他用户所看到，并且可以进行点赞、评论、转发等互动。相比与匹配后聊天的**同步互动**，基于 UGC 的点赞、评论等**异步互动**显然起到很重要的互补功能。同时，「瞬间」会以 Timeline 形式展示在个人资料卡中，这也为用户提供了一个快速深入地了解其他 Souler 的途径。

**「匿名」和「语音」是 Soul 的两个重要元素。**从「广场」、「瞬间」，到用户的个人资料卡，再到不允许用户上传自定的头像，Soul 在其每个功能角落都消灭了“用户名称”这个概念；而「语音」也贯穿于每一个用户流程之中：从匹配时可选的“语音匹配”，到聊天时的“语音聊天”，再到支持了语音内容的「广场」。通过这两个元素，用户之间就像是戴着面具在耳边低语”。在我看来这是个颇具未来感的交友场景：用户之间在感官上似乎离得很近，但实则彼此之间一无所知。这种产品设定下所营造的交友氛围是神秘而又克制的，这也使得 Soul 在一众陌生人社交软件中显得独特和出奇。

### Souler 的社交窘境

Soul 固然有许多亮点：它开辟了社交的另一种玩法，没有走基于 LBS 的陌生人社交老路，也不像 TBH 一样基于完全的匿名化的激进玩法。它完全地依赖于推荐算法来进行社交关系的探索，看似是十分可行和美好的道路，但在实际中却存在种种风险和许多亟待完善的产品逻辑。**“Souler 正处于一种社交窘境之中”——是我在深度体验了两个月产品后对当前的 Soul 的一个初步判断。** 

#### 用户社区缺乏活水

虽然 Soul 的运营现状算是稳中有升，但也一直处于一个不温不火的尴尬状态。它虽然有超过 40% 的次月留存率，但 DAU 却长期维持在三四十万的数量[^1]，可见其鼓吹的「心灵社交」并没能受到所有用户的买单。它另类的定位和小众的风格一方面缩小了目标受众的范围，另一方面让忠实用户得以圈地自萌。这种忠实用户的圈地维持着它可观的留存率的同时，也提高了新用户进入的门槛。

![](/img/in-post/2018-09-12-soulmate-at-internet-corner/soul_dau.png)

<center>    
	<div style="color:orange; border-bottom: 1px solid #d9d9d9;display: inline-block;     color: #999;padding: 1px;">Soul 日活跃用户数量趋势分析</div> 
</center>

活水的缺失对于社交软件是绝对的颓势，它应该是最需要解决、优先级最高的问题。

Soul 应该在产品与社区中强化对新用户的引导和体验保护。我曾在 Soul 社区中发起过一次小型调研，多数用户在完成了系统匹配之后会先查看匹配到的用户的时间轴，只有在时间轴中发现了他感兴趣的内容时才会主动发起聊天，这对于还未发表内容的新用户来说无疑是一种恶劣体验。

**我认为「时间轴」这个功能是可以做删减。**「时间轴」的初衷可以理解为为用户提供一个初步了解的入口，帮助陌生用户之间的“破冰”。但实际上，这个功能让用户形成了“先看动态再聊天”的用户习惯。而从社交心理的角度，未知的人与事更能引发我们的兴趣。将过于“具体”的「时间轴」更改成模糊且有限的用户画像描述，或许更能诱发聊天的产生，同时也避免了给新用户带来体验上的落差。

![](/img/in-post/2018-09-12-soulmate-at-internet-corner/soul_timeline.png)

<center>    
	<div style="color:orange; border-bottom: 1px solid #d9d9d9;display: inline-block;     color: #999;padding: 1px;">模糊化的用户描述是否更能引起聊天欲望？</div> 
</center>

#### 内容分发逻辑

Soul 当前的用户发布质量是足够优秀的，仅计算每日官方话题的用户发布率也能达到3.75%左右（在每天一个官方话题的频率下可以维持每个话题平均1.5~2万的参与度，DAU 40W）。然而这些 UGC 并没能转化为社区互动热度。分析其原因：一方面，目前大多数发布内容仍然是以文字为主，而且还存在许多大段文字，文字内容带来互动是及其有限的；另一方面，Feed 流存在许多以私人情绪为主且表意混杂的低质 UGC。

Soul 在 Feed 流上的推荐算法逻辑从体验上看“时间”是占比权重最大的因子，但是对于优质内容的引流和强化推送是缺失的。它对优质内容的引流几乎只通过在一定时间内置顶来做。对于“我”这种希望在 Feed 流看到更多优质内容的用户，只有一个置顶的优质内容是远远不足的。关于这里的内容分发该怎么做是存在权衡的：优质内容分发比例过多，会减少普通用户的流量，普通用户难以被发现；优质内容分发比例过少，则 Feed 流质量下降，用户粘性也会随之下降。

参考业内的解决方案，例如抖音是怎么做的？抖音的做法更像是**把优质内容和实时内容的比例参数化和动态化**，虽然不知道其背后的算法实现，但这种思路是可以效仿的。

### 当我们谈论陌生人社交

陌生人社交的玩法早已不是那个“左滑右滑”就可以解决的时代了，从直播，到视频聊天，再到游戏社交，各种各样的玩法和功能在陌生人社交软件里诞生和试验，说明了这个领域还存在着许多潜在的用户需求没有被挖掘和满足。

今天，当我们再次谈论起陌生人社交时，简单地套用“约炮软件”的刻板印象已经不在适用。当我们在谈论陌生人社交时，我们再也避不开以下几个课题：

1. UGC 平台：如何做一个好的 Feed 流？如何高效地分发内容？如何提高 UGC 的质量？

2. 关系的建立和维护：如何做好用户破冰？如何做有效地用户引导？如何避免用户关系下沉到微信等IM工具？

3. 用户社区的运营：如何提高用户的互动热度？如何营造符合产品气质的用户社区氛围？

4. 安全监管：如何过滤有风险的用户内容？如何提高平台的监管力度？

   ......

张小龙曾在饭否上说：互联网的最终目的，是让关系学见鬼去。[^2]我想如果有一个互联网产品能深刻地改变关系学，那它一定不会是像微信一般用于“维护关系”的 IM 工具，更有可能地，它的形态会更接近于以“探索关系”和“建立关系”为使命的陌生人社交。我期待着见证这样一款改变关系学的互联网产品的诞生。



[^1]: Soul 运营数据来自易观千帆。
[^2]: 引自看完了张小龙的 2359 条饭否日记，https://zhuanlan.zhihu.com/p/20539834。