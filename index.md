---
title: Home
layout: home
---
# 병신같이 질문하지 않는 법

영어 원제 : How To Ask Questions The Smart Way
----------------------------------

### 저자 및 역자

### Eric Steven Raymond

[Thyrsus Enterprises](http://www.catb.org/~esr/)  

[esr@thyrsus.com](mailto:esr@thyrsus.com)

### Rick Moen

[respond-auto@linuxmafia.com](mailto:respond-auto@linuxmafia.com)  

Copyright © 2001,2006,2014 Eric S. Raymond, Rick Moen

### 전웅배 (한국어 번역자)

[woongbae@unist.ac.kr](https://wbjeon2k.github.io/about)

**목차 Table of Contents**

[번역본](#번역본)

[경고문](#경고문)

[서론](#서론)

[질문을 하기에 앞서서](#질문을-하기에-앞서서)

[질문을 할 때](#질문을-할-때)

[질문하려는 포럼을 신중히 고르세요](#forum)

[Stack Overflow](#stackoverflow)

[웹 및 IRC 포럼](#usefora)

[프로젝트 메일링 리스트는 차선책으로](#uselists)

[Use meaningful, specific subject headers](#bespecific)

[Make it easy to reply](#easyreply)

[Write in clear, grammatical, correctly-spelled language](#writewell)

[Send questions in accessible, standard formats](#formats)

[Be precise and informative about your problem](#beprecise)

[Volume is not precision](#volume)

[Don't rush to claim that you have found a bug](#idm368)

[Grovelling is not a substitute for doing your homework](#idm379)

[Describe the problem's symptoms, not your guesses](#symptoms)

[Describe your problem's symptoms in chronological order](#chronology)

[Describe the goal, not the step](#goal)

[Don't ask people to reply by private e-mail](#noprivate)

[Be explicit about your question](#explicit)

[When asking about code](#code)

[Don't post homework questions](#homework)

[Prune pointless queries](#prune)

[Don't flag your question as “Urgent”, even if it is for you](#urgent)

[Courtesy never hurts, and sometimes helps](#courtesy)

[Follow up with a brief note on the solution](#followup)

[How To Interpret Answers](#answers)

[RTFM and STFW: How To Tell You've Seriously Screwed Up](#rtfm)

[If you don't understand...](#lesser)

[Dealing with rudeness](#keepcool)

[On Not Reacting Like A Loser](#not_losing)

[Questions Not To Ask](#classic)

[Good and Bad Questions](#examples)

[If You Can't Get An Answer](#idm659)

[How To Answer Questions in a Helpful Way](#idm667)

[Related Resources](#idm690)

[Acknowledgements](#idm696)

[Revision History](#revision-history)

역자의 서문
------------
역자는 전문 번역가가 아니며, 심심해서 본 문서를 번역 하였습니다.  

본 문서는 2004년에 처음 작성 되었습니다.  
따라서 2022년 현재와 다른 환경(메일링 리스트, 뉴스그룹 등)을 기반으로 하고 있습니다.  
시간이 지나도 변하지 않는 본질적인 내용에 초점을 맞추어 읽어주시면 감사하겠습니다.  

다소 과격한 어휘의 사용은 원래 영어 본문에서 전달하려는 시니컬 하면서도 친절한 느낌을 살리기 위함을 알립니다.  
번역에 수정 사항을 제안하고 싶으시다면 PR이나 이슈를 남겨주세요.  

맞춤법 검사기는 해당 링크의 검사기를 사용 하였습니다. [맞춤법검사기](http://speller.cs.pusan.ac.kr/results)  
맞춤법이 많이 틀려서 읽기 불편 하시다면, 더 좋은 검사기로 고치도록 하겠습니다.

번역본
------------

번역본들: [Original English](http://www.catb.org/~esr/faqs/smart-questions.html) [Brazilo-Portuguese](http://blogofscience.com/perguntas.html) [Chinese (Traditional)](https://github.com/ryanhanwu/How-To-Ask-Questions-The-Smart-Way) [Czech](http://scientificachievements.com/jak-se-ptat-chytry-zpusob/) [Dutch](http://docs.jaspervries.nl/smart-questions/) [Estonian](http://glory4cars.com/edu/kuidas-esitada-kusimusi-nutikas-viis/) [French](http://www.gnurou.org/documents/smart-questions-fr.html) [Georgian](http://maxo127.narod.ru/Geo/Articles/smart-questions_ge.html) [German](https://www.privatkreditsofort.ch/wie-man-fragen-richtig-stellt/) [Greek](http://www.dionyziz.com/howto-smart-questions-gr/) [Hindi](http://kntuniversity.org/how-to-ask-questions-the-smart-way/) [Hungarian](http://www.forallworld.com/milyen-kerdeseket-okosan/) [Indonesion](https://www.chameleonjohn.com/translations/smart-questions-Indonesian) [Japanese](http://www.ranvis.com/articles/smart-questions.ja.html) [Lithuanian](http://myscres.com/articles/kaip-uzduoti-klausimus-protinga-buda.html) [Polish](http://rtfm.killfile.pl) [Portuguese](https://www.homeyou.com/~edu/perguntar-de-forma-inteligente) [Russian](http://maddog.sitengine.ru/smart-question-ru.html) [Spanish](http://www.sindominio.net/ayuda/preguntas-inteligentes.html) [Ukrainian](http://eustudiesweb.com/yak-staviti-zapitannya-rozumno/) [Uzbek](http://www.bestcarzin.com/blog/smart-questions-uzb/)  
If you want to copy, mirror, translate, or excerpt this document, please see my [copying policy](http://www.catb.org/~esr/copying.html).

경고문
----------

<!-- Many project websites link to this document in their sections on how to get help. That's fine, it's the use we intended — but if you are a webmaster creating such a link for your project page, please display prominently near the link notice that _we are not a help desk for your project!_ -->

많은 프로젝트 페이지가 도움을 얻기 위한 방법을 안내하는 섹션에서 본 문서를 링크합니다.  
그것이 본 문서의 목적이기는 하다 마는 - 이 글을 보는 당신이 본 문서로 안내 링크를 거는 프로젝트의 웹 마스터라면,  
해당 링크 옆에 잘 보이도록 아래 경고문을 꼭 써주세요.  
**"!!여기는 당신네 프로젝트를 위한 안내 데스크가 아닙니다!!"**

<!-- We have learned the hard way that without such a notice, we will repeatedly be pestered by idiots who think having published this document makes it our job to solve all the world's technical problems. -->

위 경고문이 없다면, 우리(*역주 : 원저자들*)는 본 문서를 작성했다는 이유 하나만으로 전 세계의 모든 기술적인 문제들을 해결하는 것이 우리의 일인 것처럼 착각하는 멍청이들로부터 고통을 받는다는 사실을 쓰라린 과정을 통해서 알아내었습니다.

<!-- If you're reading this document because you need help, and you walk away with the impression you can get it directly from the authors of this document, _you_ are one of the idiots we are talking about. -->
도움이 필요해서 이 글을 읽으러 오신 분 중에서 이 글을 읽고 본 문서를 적은 저자들로부터 직접적인 도움을 받을 수 있겠다고 생각하셨다면, **당신은** 바로 우리가 말하는 멍청이 중 하나입니다.
<!-- Don't ask _us_ questions. We'll just ignore you. We are here to show you how to get help from people who actually know about the software or hardware you're dealing with, but 99.9% of the time that will not be us. -->
**저자들에게** 질문을 하지 마세요. 우리는 그냥 당신 요청을 무시할 겁니다. 우리는 당신들이 도움을 필요로 하는 SW나 HW를 잘 알고 있는 사람들로부터 도움을 받는 법을 보여주기 위해 문서를 작성하였고, 99.9%의 경우에는 우리는 도움을 줄 수 있는 사람이 아닙니다.
<!-- Unless you know for _certain_ that one of the authors is an expert on what you're dealing with, leave us alone and everybody will be happier. -->
저자 중 한 명이 당신의 문제를 겪고 있는 사항에 대한 전문가라는 사실을 **확실히** 아는 것이 아니라면, 모두의 행복을 위해서라도 우리를 괴롭히지 말아 주세요.

(*역주 : 번역자에게도 질문 금지입니다*)

서론
------------

<!-- In the world of [hackers](http://www.catb.org/~esr/faqs/hacker-howto.html), the kind of answers you get to your technical questions depends as much on the way you ask the questions as on the difficulty of developing the answer. -->
이쪽 [해커](http://www.catb.org/~esr/faqs/hacker-howto.html)들의 바닥에서는, 여러분들이 가진 기술적인 문제에 대한 답변을 받기 위해 질문을 하는 방법이 해당 질문의 난이도만큼이나 중요합니다.  
(*역주 : 본 문서에서 '해커'는 '전문가'의 의미에 더 가깝습니다. 초보자(newbie) 의 반대.*)
<!-- This guide will teach you how to ask questions in a way more likely to get you a satisfactory answer. -->
본 가이드는 여러분들이 더욱더 높은 확률로 만족스러운 답변을 받기 위해서 질문을 제대로 하는 법을 가르쳐 드릴 겁니다.

<!-- Now that use of open source has become widespread, you can often get as good answers from other, more experienced users as from hackers. -->
오늘날에는 오픈소스가 널리 보급되어서, 숙련된 해커들 뿐만 아니라 경험이 풍부한 사용자들로 부터도 종종 좋은 답을 얻을 수 있습니다.
<!-- This is a Good Thing; users tend to be just a little bit more tolerant of the kind of failures newbies often have. -->
이는 좋은 현상입니다. 사용자들은 해커들 보다 대체로 뉴비들이 겪는 문제들에 대해서 조금 더 인내심을 발휘하는 편 입니다.

<!-- Still, treating experienced users like hackers in the ways we recommend here will generally be the most effective way to get useful answers out of them, too. -->
하지만, 경험이 풍부한 사용자들 에게도 본 문서에서 안내하는 숙련된 해커에게 질문 하는 법을 그대로 사용하는 것이 일반적으로는 여전히 제일 효과적입니다.

<!-- The first thing to understand is that hackers actually like hard problems and good, thought-provoking questions about them. If we didn't, we wouldn't be here. -->
모든 것에 앞서서 하나 이해를 해야하는 것은, 해커들은 사실 어려운 문제들과 그 문제들에 대한 수준 높은, 생각을 많이 필요로 하는 질문을 좋아합니다. 그렇지 않다면, 우리는 이 자리에 있지 않을 것입니다.

<!-- If you give us an interesting question to chew on we'll be grateful to you; good questions are a stimulus and a gift. Good questions help us develop our understanding, and often reveal problems we might not have noticed or thought about otherwise. Among hackers, “Good question!” is a strong and sincere compliment. -->
여러분이 우리 해커들에게 뜯고 씹고 맛보고 즐길만한 좋은 질문거리를 던져 주신다면 정말 감사하겠습니다. 좋은 질문은 자극제 이며 일종의 선물입니다. 좋은 질문들은 우리 스스로가 가진 이해의 폭을 넓히며, 질문을 보지 않았다면 무심코 지나쳤거나 떠올리지 못했을 주제에 대한 문제를 새로이 밝혀냅니다. 해커들의 세계에서는, "좋은 질문이네요!" 라는 말은 강력하고도 진실된 칭찬입니다.

<!-- Despite this, hackers have a reputation for meeting simple questions with what looks like hostility or arrogance. It sometimes looks like we're reflexively rude to newbies and the ignorant. But this isn't really true. -->
그런데도, 해커들은 간단한 질문들에 대해서는 적대적이거나 건방지게 대한다는 나쁜 평판을 가지고 있습니다. 이는 때때로 우리들이 무조건 초심자들이나 무지한 사람들에게 못되게 구는 것처럼 보여지게 합니다. 하지만 이것은 사실이 아닙니다.

<!-- What we are, unapologetically, is hostile to people who seem to be unwilling to think or to do their own homework before asking questions.
People like that are time sinks — they take without giving back, and they waste time we could have spent on another question more interesting and another person more worthy of an answer. We call people like this “losers” (and for historical reasons we sometimes spell it “lusers”). -->
우리는 질문을 하기 전에 아무 생각도 하기 싫어하거나, 질문을 하기 전에 자기가 스스로 해야 하는 일들을 하지 않고 질문하는 사람들에게 적대적으로 굽니다. 그리고 여기에 대해서는 전혀 미안한 마음이 없습니다. 그런 사람들은 시간을 잡아먹기만 합니다. 그 사람들은 도움을 받기만 하고 다시 돌려주는 법이 없으며, 더 흥미로운 질문이나 더욱 도움이 필요한 사람들에게 사용될 수 있었던 시간을 낭비하게 만듭니다. 우리는 이런 사람들을 “병신(loser)”이라고 부릅니다. ( 또한 과거부터 쌓인 여러 이유로 우리는 때때로 이 사람들을 "lusers" 라고도 부릅니다.)
(*역주 : "lusers" 는 "loser" + "user" 로, 해커들의 slang 입니다. ["lusers"](https://en.wiktionary.org/wiki/luser)*)

<!-- We realize that there are many people who just want to use the software we write, and who have no interest in learning technical details. For most people, a computer is merely a tool, a means to an end; they have more important things to do and lives to live. We acknowledge that, and don't expect everyone to take an interest in the technical matters that fascinate us. Nevertheless, our style of answering questions is tuned for people who _do_ take such an interest and are willing to be active participants in problem-solving. That's not going to change. Nor should it; if it did, we would become less effective at the things we do best. -->
우리는 우리들이 만든 소프트웨어의 기술적인 디테일에는 전혀 관심이 없고 그냥 갖다 쓰고만 싶은 사람들이 정말 많다는 것을 깨달았습니다. 대부분의 사람들에게 있어서 컴퓨터는 그냥 도구일 뿐, 그 이상의 의미는 없습니다. 그 사람들은 인생에 있어서 더 중요한 게 있는 것이겠죠. 우리 해커들은 그 사실을 받아들이며, 우리는 모든 사람이 우리들이 재미있어하는 기술적인 주제들에 대해서 재미를 가질 것이라 기대하지 않습니다. 그런데도, 우리들이 사용하는 답변 양식은 기술적인 주제들에 관해 **관심이 있으며**, 적극적으로 문제를 해결하고자 하는 사람들에게 맞춰져 있습니다. 이것은 앞으로도 변하지 않을 사실이며, 바뀌어서도 안 됩니다. 그렇지 않았다면, 우리는 우리가 제일 잘하는 이 일을 더 잘하지 못하게 되었을 것입니다.

<!-- We're (largely) volunteers. We take time out of busy lives to answer questions, and at times we're overwhelmed with them. So we filter ruthlessly. In particular, we throw away questions from people who appear to be losers in order to spend our question-answering time more efficiently, on winners. -->
우리들은 (대부분) 자원봉사자들입니다. 우리는 각자 바쁜 시간을 쪼개서 질문에 대답하며, 때로는 대답하기가 벅찰 정도입니다. 따라서 우리는 가차 없이 질문들을 걸러냅니다. 특히나 우리는 똘똘한 친구들에게 우리들이 질문을 대답하는 데 사용할 수 있는 시간을 효율적으로 쓰기 위해서, 병신같은 사람들의 질문은 갖다 버려버립니다.

<!-- If you find this attitude obnoxious, condescending, or arrogant, check your assumptions. We're not asking you to genuflect to us — in fact, most of us would love nothing more than to deal with you as an equal and welcome you into our culture, if you put in the effort required to make that possible. But it's simply not efficient for us to try to help people who are not willing to help themselves. It's OK to be ignorant; it's not OK to play stupid. -->
이 글을 읽는 여러분들 중 이런 우리들의 태도가 매우 불쾌하거나, 업신여기며 잘난 체 하는 듯 보이거나, 건방지다고 느껴진다면 여러분들의 생각을 다시 돌이켜 볼 필요가 있습니다. 우리는 여러분들이 우리에게 굽실거리는 것을 바라는 게 전혀 아닙니다. 사실은, 우리 중 대부분의 사람은 여러분들과 동등한 관계를 맺고, 우리들의 문화에 맞추려고 노력하는 사람들은 더욱 환영합니다. 다만 스스로를 도울 생각이 전혀 없는 사람들을 도우려고 하는 것은 효율적이지 못할 뿐입니다. 잘 모르는 건 괜찮습니다. 하지만 멍청한 짓을 하는 건 괜찮지 않습니다.

<!-- So, while it isn't necessary to already be technically competent to get attention from us, it _is_ necessary to demonstrate the kind of attitude that leads to competence — alert, thoughtful, observant, willing to be an active partner in developing a solution. If you can't live with this sort of discrimination, we suggest you pay somebody for a commercial support contract instead of asking hackers to personally donate help to you. -->
우리의 관심을 받기 위해서 기술적인 능력이 출중할 필요는 없습니다. 하지만 출중한 능력을 키우는데 필요한 태도들은 꼭 필요합니다. 기민함, 깊이있게 생각 하는 것, 관찰력, 해결 방법을 찾는 데 있어서 적극적으로 참여하려는 태도 등을 의미합니다. 이런 방식들이 영 맞지 않는 사람들은 해커들에게 재능 기부를 요구하기보다는, 그냥 돈을 내고 사후 지원을 받기를 바랍니다.

<!-- If you decide to come to us for help, you don't want to be one of the losers. You don't want to seem like one, either. The best way to get a rapid and responsive answer is to ask it like a person with smarts, confidence, and clues who just happens to need help on one particular problem. -->
이 글을 읽는 당신이 우리들을 도와주기로 결심하셨다면, 당신은 병신 중 한 명이 되어서는 안 됩니다. 병신같은 인상을 풍겨서도 안 됩니다. 빠르고 적극적인 대답을 받는 데 있어서 가장 좋은 방법은 똑똑하고 자신감 있으며, 도움을 주려는 사람들이 문제를 특정하여 파악할 수 있는 내용들을 가지고 있는 사람들과 같이 질문을 하는 겁니다.

<!-- (Improvements to this guide are welcome. You can mail suggestions to [esr@thyrsus.com](mailto:esr@thyrsus.com) or [respond-auto@linuxmafia.com](mailto:respond-auto@linuxmafia.com). Note however that this document is not intended to be a general guide to [netiquette](http://www.ietf.org/rfc/rfc1855.txt), and we will generally reject suggestions that are not specifically related to eliciting useful answers in a technical forum.) -->
(본 가이드를 개정하기 위한 도움은 환영합니다. [esr@thyrsus.com](mailto:esr@thyrsus.com) 또는 [respond-auto@linuxmafia.com](mailto:respond-auto@linuxmafia.com)에 이메일로 제안을 하실 수 있습니다. 본 문서는 일반적인 [네티켓](http://www.ietf.org/rfc/rfc1855.txt)에 관한 안내가 아니기에, 기술적인 포럼에서 유용한 대답을 끌어내는 방법과 관련이 없는 내용들은 보내지 말아 주세요.)

<div id='질문을-하기에-앞서서'/>  

질문을 하기에 앞서서
--------------

<!-- Before asking a technical question by e-mail, or in a newsgroup, or on a website chat board, do the following: -->
기술적인 문제에 대해 이메일, 뉴스 그룹, 인터넷 게시판 등에 질문을 하기 전에, 아래 사항들을 미리 하세요 :

<!-- 1. Try to find an answer by searching the archives of the forum or mailing list you plan to post to. -->
1. 질문을 올리려고 하는 포럼에 이미 올라왔던 자료들에서 답을 찾으려고 해보세요.  

<!-- 2. Try to find an answer by searching the Web. -->
2. 인터넷 검색을 해보세요.

<!-- 3. Try to find an answer by reading the manual. -->
3. 매뉴얼/공식 문서를 읽어보세요.

<!-- 4. Try to find an answer by reading a FAQ. -->
4. 자주 묻는 질문(FAQ) 를 읽어보세요.

<!-- 5. Try to find an answer by inspection or experimentation. -->
5. 직접 문제를 분석 하거나 실험을 해보면서 답을 찾으려고 해보세요.

<!-- 6. Try to find an answer by asking a skilled friend. -->
6. 실력 있는 친구에게 물어보세요.

<!-- 7. If you're a programmer, try to find an answer by reading the source code. -->
7. 당신이 진짜 프로그래머 라면, 소스코드를 읽어서 직접 답을 찾아보려고 하세요.

<!-- When you ask your question, display the fact that you have done these things first; this will help establish that you're not being a lazy sponge and wasting people's time. Better yet, display what you have _learned_ from doing these things. We like answering questions for people who have demonstrated they can learn from the answers. -->
질문을 할 때, 위 사항들에서 제시한 문제를 해결하려는 방법들을 시도해 봤다는 것을 보여줘야 합니다. 시도한 것을 보여 줘야 당신이 게을러터진 사람이 아니며, 사람들의 시간을 낭비하려는 게 아니라는 걸 증명할 수 있습니다. 더 좋은 방법은, 당신이 문제를 해결하려는 과정에서 **무엇을 배웠는지**도 같이 보여주세요. 우리는 우리의 답변을 통해 무언가를 배울 수 있는 사람들에게 답변하는 것을 좋아합니다.

<!-- Use tactics like doing a Google search on the text of whatever error message you get (searching [Google groups](http://groups.google.com/) as well as Web pages). This might well take you straight to fix documentation or a mailing list thread answering your question. Even if it doesn't, saying “I googled on the following phrase but didn't get anything that looked promising” is a good thing to do in e-mail or news postings requesting help, if only because it records what searches won't help. It will also help to direct other people with similar problems to your thread by linking the search terms to what will hopefully be your problem and resolution thread. -->
여러분들이 맞닥뜨린 에러 메시지에 대해서 Google 검색을 해보세요. ([Google groups](http://groups.google.com/)와 웹 페이지를 찾는 것을 모두 포함합니다.). 이 방법은 해결 방법이 적힌 문서나 댓글 스레드에 여러분들을 바로 데려다줄 수도 있습니다. 검색해서 나오지 않더라도, "구글에 해당 문구로 검색을 해봤는데 도움이 될만한 내용이 없었습니다."라는 말을 질문 글에 넣는다면, 다른 사람들이 해당 방법으로 검색하면 답을 찾을 수 없다는 것을 알려줄 수 있기에 도움이 됩니다. 또한, 이는 비슷한 문제를 가진 다른 사람들이 당신이 남긴 글을 통해 문제를 해결할 수도 있는 자료에 접근하는 것을 도와줄 수 있습니다.

<!-- Take your time. Do not expect to be able to solve a complicated problem with a few seconds of Googling. Read and understand the FAQs, sit back, relax and give the problem some thought before approaching experts. Trust us, they will be able to tell from your questions how much reading and thinking you did, and will be more willing to help if you come prepared. Don't instantly fire your whole arsenal of questions just because your first search turned up no answers (or too many). -->
충분히 시간을 두고 찾아보세요. 어려운 문제에 대한 답을 구글링 몇 초 찔끔해서 찾을 수 있으리라 기대하지는 마세요. FAQ들을 읽고 이해를 한 다음 가만히 앉아서 문제에 대한 생각을 곰곰이 해 본 다음에 전문가들에게 물어보려고 하세요. 우리가 제시한 방법을 믿어보세요. 전문가들은 여러분들이 하는 질문을 통해서 여러분들이 문제에 대해서 얼마나 생각을 해봤는지, 얼마나 자료를 읽어봤는지 대번에 알 수 있습니다. 또한 전문가들은 준비해 온 사람들을 더 도와주고 싶어 합니다. 처음 한 번 검색해보고 아무 답을 찾을 수 없다고 (또는 너무 많은 답이 있어서 헷갈린다고) 여러분의 질문들을 와르르 쏟아내지 마세요.

<!-- Prepare your question. Think it through. Hasty-sounding questions get hasty answers, or none at all. The more you do to demonstrate that having put thought and effort into solving your problem before seeking help, the more likely you are to actually get help. -->
질문할 내용을 잘 정리해서 질문할 준비를 하세요. 질문에 대해서 곰곰이 생각을 해보세요. 대충 적은 것 같은 질문은 답변도 대충 받거나, 아니면 아무 답변을 받을 수 없습니다. 도움을 요청하기 전에 여러분들이 문제를 해결하기 위해서 생각을 충분히 하고, 상당한 노력을 했다는 걸 보여줄수록 실질적으로 도움이 되는 답변을 받을 확률이 높습니다.

<!-- Beware of asking the wrong question. If you ask one that is based on faulty assumptions, J. Random Hacker is quite likely to reply with a uselessly literal answer while thinking “Stupid question...”, and hoping the experience of getting what you asked for rather than what you needed will teach you a lesson. -->
잘못된 질문을 하지 않도록 조심하세요. 잘못된 전제 조건을 바탕으로 한 질문을 하게 된다면, 임의의 해커 Gildong Hong 씨는 그다지 쓸모가 없을 정도로 당연한 답변을 달면서 속으로 "병신같은 질문이군..." 이란 생각을 할 겁니다. 또한 여러분들이 한 질문에 대한 답변이 여러분들이 필요로 했던 답변이 아니라는 사실을 알게 되실 겁니다.

<!-- Never assume you are _entitled_ to an answer. You are not; you aren't, after all, paying for the service. You will earn an answer, if you earn it, by asking a substantial, interesting, and thought-provoking question — one that implicitly contributes to the experience of the community rather than merely passively demanding knowledge from others. -->
답변을 반드시 받아야 할 권리가 있다고 **착각하지 마세요**. 당신에게는 그런 권리가 없습니다. 당신은 답변받기 위해서 돈 내는 것도 아닌걸요. 당신은 중요성이 높고, 흥미로우며, 생각을 불러일으키는 좋은 질문을 해야 답변을 얻어낼 수 있습니다. 답변받을 만한 가치가 있는 좋은 질문들은 다른 사람들이 알고 있는 것을 수동적으로 받아내려고만 하는 게 아니라, 우리 커뮤니티의 발전에 도움을 주는 질문들입니다.

<!-- On the other hand, making it clear that you are able and willing to help in the process of developing the solution is a very good start. “Would someone provide a pointer?”, “What is my example missing?”, and “What site should I have checked?” are more likely to get answered than “Please post the exact procedure I should use.” because you're making it clear that you're truly willing to complete the process if someone can just point you in the right direction. -->
한 편으로는, 당신이 해답을 만들 능력이 있거나, 만들려는 의지가 있다는 것을 확실히 보여주는 것은 답변을 만들어 가는 데 있어서 매우 좋은 시작점입니다. "어디를 찾아봐야 하는지 포인터를 알려주실 수 있나요?", "예시에서 빠뜨린 것이 있나요?", "어느 사이트에서 찾아보면 좋을까요?"와 같은 질문들은 "내가 뭘 어떻게 해야 하는지 정확히 다 알려주세요" 따위의 질문보다는 답변받을 가능성이 높습니다. 왜냐하면 당신은 방향만 잘 잡아준다면 해답을 찾아 나설 의지가 있다는 것을 보여주었기 때문입니다.

<div id='질문을-할-때'/>

질문을 할 때
------------


<!-- ### Choose your forum carefully -->
### 질문하려는 포럼을 신중히 고르세요

<div id='forum'/>

<!-- Be sensitive in choosing where you ask your question. You are likely to be ignored, or written off as a loser, if you:

* post your question to a forum where it's off topic

* post a very elementary question to a forum where advanced technical questions are expected, or vice-versa

* cross-post to too many different newsgroups

* post a personal e-mail to somebody who is neither an acquaintance of yours nor personally responsible for solving your problem -->
어디에 질문을 하려고 하는지 신경을 써서 골라야 합니다. 당신은 아래와 같은 짓을 하면 무시당하거나 병신 취급을 받을 겁니다. 만약…

* 질문하려는 주제와 맞지 않는 포럼에 질문을 올리는 경우

* 지식수준이 어느 정도 이상 갖춰진 전문적인 질문을 올리는 포럼에 너무 기초적인 질문을 하거나, 반대로 기초적인 질문을 하는 포럼에 너무 전문적인 질문을 하는 경우

* 여러 뉴스그룹에 같은 질문을 중복하여 너무 많이 올리는 경우

* 안면이 있는 사람이 아니거나, 당신의 질문에 반드시 개인적으로 답변을 해 주어야 할 의무가 없는 사람들에게 이메일 주소를 적어놓고 메일로 답변을 요구하는 경우

<!-- Hackers blow off questions that are inappropriately targeted in order to try to protect their communications channels from being drowned in irrelevance. You don't want this to happen to you. -->
해커들은 잘못 들어온 질문들을 쳐냅니다. 이는 해커들의 커뮤니티 채널이 관련 없는 내용들로 넘치는 것을 막기 위함입니다. 여러분들도 본인에게 그런 일이 발생하는 건 원하지 않을 겁니다.

<!-- The first step, therefore, is to find the right forum. Again, Google and other Web-searching methods are your friend. Use them to find the project webpage most closely associated with the hardware or software giving you difficulties. Usually it will have links to a FAQ (Frequently Asked Questions) list, and to project mailing lists and their archives. These mailing lists are the final places to go for help, if your own efforts (including _reading_ those FAQs you found) do not find you a solution. The project page may also describe a bug-reporting procedure, or have a link to one; if so, follow it. -->
그러므로 질문을 하는 데 있어서 가장 먼저 해야 하는 것은 적절한 포럼을 찾는 겁니다. 다시 말씀드리지만, 구글과 다른 인터넷 검색 도구들은 당신들의 친구랍니다. 당신이 문제를 겪고 있는 SW나 HW와 가장 밀접한 관련이 있는 프로젝트 웹페이지를 찾기 위해서 검색을 하세요. 보통은 FAQ(자주 하는 질문) 목록이나 프로젝트 관련 연락처 목록, 프로젝트 아카이브 등에 대한 링크를 찾을 수 있습니다. 프로젝트 관련 연락처(mailing list)로 문의를 하는 것은 여러분들이 스스로 문제를 해결하려고 노력(*FAQ를 읽는 등*)해보고도 해결을 할 수 없다면 마지막으로 써야 하는 방법입니다. 해당 프로젝트 페이지에는 버그를 신고하는 절차가 적혀있거나, 신고하는 링크가 달린 경우가 있습니다. 그렇다면, 해당 링크를 참고하세요.

<!-- Shooting off an e-mail to a person or forum which you are not familiar with is risky at best. For example, do not assume that the author of an informative webpage wants to be your free consultant. Do not make optimistic guesses about whether your question will be welcome — if you're unsure, send it elsewhere, or refrain from sending it at all. -->
기존에 면식이 없던 사람이나 포럼에 질문을 난사하는 건 잘 쳐줘도 확률이 낮은 방법입니다. 예를 들어서, 알찬 정보가 들어있는 웹페이지를 작성한 사람이 당신의 무료 컨설턴트가 되어줄 것으로 생각하지 마세요. 당신의 질문이 환영받으리라고 낙관적으로 생각하지 마세요. 환영받을지 잘 모르겠다면 다른 곳에 질문을 보내거나, 질문을 보내는 것을 처음부터 삼가는 것이 좋습니다.

<!-- When selecting a Web forum, newsgroup or mailing list, don't trust the name by itself too far; look for a FAQ or charter to verify your question is on-topic. Read some of the back traffic before posting so you'll get a feel for how things are done there. In fact, it's a very good idea to do a keyword search for words relating to your problem on the newsgroup or mailing list archives before you post. It may find you an answer, and if not it will help you formulate a better question. -->
인터넷 포럼, 뉴스그룹, 메일링 리스트 등을 선택할 때 단체의 이름을 너무 믿지는 마세요. FAQ나 운영 안내문을 찾아서 당신이 하려는 질문의 주제와 부합하는지 확인하세요. 새로운 게시물을 올리기 전에 과거 게시물들을 보면서 게시판이 어떻게 굴러가는지 감을 잡아보세요. 사실 질문을 하기 전에, 당신의 문제와 관련된 키워드를 뉴스그룹이나 메일링 리스트 과거 기록에서 찾아보는 건 매우 좋은 생각입니다. 당신이 원하는 답을 찾을 수도 있고, 그렇지 않더라도 더 나은 질문을 작성하는 데 도움이 됩니다.

<!-- Don't shotgun-blast all the available help channels at once, that's like yelling and irritates people. Step through them softly. -->
모든 채널에다가 당신이 하고 싶은 말을 도배하듯 쏟아내지 마세요. 그건 마치 사람들에게 소리를 지르는 것과 같고 다른 사람들을 불편하게 만듭니다. 부드럽게 다가가세요.

<!-- Know what your topic is! One of the classic mistakes is asking questions about the Unix or Windows programming interface in a forum devoted to a language or library or tool portable across both. If you don't understand why this is a blunder, you'd be best off not asking any questions at all until you get it. -->
당신이 말하려고 하는 문제의 주제(topic)에 대해서 파악하세요! 흔히 발생하는 실수 중 하나는, Unix와 Windows에 모두 호환되는 언어/라이브러리/툴을 위해 유지되는 포럼에다 Unix/Windows programming interface에 관한 질문을 하는 겁니다. 당신이 이게 왜 잘못된 행동인지 이해를 할 수 없다면, 이해될 때까지 아무 질문도 하지 않는 것이 상책입니다.

<!-- In general, questions to a well-selected public forum are more likely to get useful answers than equivalent questions to a private one. There are multiple reasons for this. One is simply the size of the pool of potential respondents. Another is the size of the audience; hackers would rather answer questions that educate many people than questions serving only a few. -->
일반적으로는, 공개적으로 활동하는 포럼이 폐쇄적으로 활동하는 포럼보다 같은 질문을 했을 때 도움이 되는 답변을 받는 경우가 많습니다. 한 가지 이유는 질문에 대답해줄 수 있는 사람들의 수가 많기 때문입니다. 다른 이유는 질문을 보는 사람들의 수도 많기 때문입니다. 해커들은 일부 사람들에만 도움이 되는 질문보다, 많은 사람에게 도움을 줄 수 있는 질문에 대답하려고 하기 때문입니다.

<!-- Understandably, skilled hackers and authors of popular software are already receiving more than their fair share of mis-targeted messages. By adding to the flood, you could in extreme cases even be the straw that breaks the camel's back — quite a few times, contributors to popular projects have withdrawn their support because collateral damage in the form of useless e-mail traffic to their personal accounts became unbearable. -->
당연하게도, 실력 있는 해커들이나 인기 있는 소프트웨어 제작자들은 지금도 목적지가 잘못된 메시지들을 필요 이상으로 많이 받고 있습니다. 당신이 이 잘못된 메시지들의 범람에 거들게 된다면, 극단적인 경우에는 무거운 짐을 짊어진 낙타의 등을 부러뜨리는 마지막 밀짚 한 줄기가 당신의 메시지가 될 수도 있습니다. 인기 있는 프로젝트의 기여자들이 개인 계정에 도저히 참을 수 없을 정도로 많은 양의 쓸모없는 이메일들이 쏟아져서 심각한 지장을 겪고 프로젝트 지원을 그만두는 일이 종종 발생합니다.

<div id='stackoverflow'/>

### Stack Overflow

<!-- Search, _then_ ask on Stack Exchange -->
**먼저 검색을 해보고** Stack Exchange에 물어보세요.

<!-- In recent years, the Stack Exchange community of sites has emerged as a major resource for answering technical and other questions and is even the preferred forum for many open-source projects. -->
근 몇 년 사이에, Stack Exchange는 기술적인 주제들을 포함한 여러 질문에 답변을 다는 주요 커뮤니티로 성장을 하였으며, 심지어 많은 오픈소스 프로젝트는 Stack Exchange 포럼을 선호합니다.

<!-- Start with a Google search before looking at Stack Exchange; Google indexes it in real time. There's a very good chance someone has already asked a similar question, and the Stack Exchange sites are often near the top of the search results. If you didn't find anything through Google, search again on the specific site most relevant to your question (see below). Searching with tags can help narrow down the results. -->
Stack Exchange를 들여다보기 전에 Google 검색을 먼저 해보세요. Google은 실시간으로 페이지들을 정리한답니다. 매우 높은 확률로 다른 사람이 이미 비슷한 질문을 했을 수도 있고, 상위 검색 결과에 Stack Exchange 사이트들이 표시되는 경우가 대부분입니다. 구글 검색을 통해서 아무것도 찾을 수 없었다면, 당신의 질문과 가장 밀접한 주제를 구체적으로 다루는 사이트에서 다시 찾아보세요. (사이트들의 목록은 아래를 참조하세요.) 태그와 함께 검색하는 것은 검색 결과들을 좁히는 데 도움이 됩니다.

<!-- If you still didn't find anything, post your question on the _one_ site where it's most on-topic. Use the formatting tools, especially for code, and add tags that are related to the substance of your question (particularly the name of the programming language, operating system, or library you're having trouble with). If a commenter asks you for more information, edit your main post to include it. If any answer is helpful, click the up arrow to upvote it; if an answer gives a solution to your problem, click the check under the voting arrows to accept it as correct. -->
여전히 아무것도 찾을 수 없다면, 질문과 가장 관련이 깊은 *한 개*의 사이트에 질문을 올리세요. 특히 코드를 올릴 때는 코드 양식을 정리해주는 도구들(formatting tools)을 사용하고, 당신의 질문과 가장 관련이 있는 용어들을 태그로 달아두세요. (구체적인 예시로는, 당신이 문제를 겪고 있는 프로그래밍 언어, OS, 혹은 라이브러리 등입니다.) 댓글을 단 사람이 답변을 위해 더 많은 정보를 요청한다면, 원 글을 수정하여 추가 정보들을 반영하세요. 도움이 된 답변에는 추천(upvote)을 눌러주세요. 어떤 답변이 직접적으로 문제를 해결하는 데 도움을 주었다면, 추천 화살표 밑에 있는 체크 버튼을 눌러서 올바른 답변임을 확인 해주세요.

<!-- Stack Exchange has grown to [over 100 sites](http://stackexchange.com/sites), but here are the most likely candidates: -->
Stack Exchange는 [100개가 넘는 사이트들](http://stackexchange.com/sites)로 성장 했습니다. 아래는 제일 유용할 후보군들입니다.

<!-- * Super User is for questions about general-purpose computing. If your question isn't about code or programs that you talk to only over a network connection, it probably goes here. -->
* Super User는 컴퓨터 사용과 관련된 일반적인 질문들을 위한 사이트입니다. 구체적인 코드나 프로그램에 관한 내용이 아니라 그냥 인터넷 연결 정도에 관한 질문이라면, 아마 여기로 가는 게 맞을 겁니다.

<!-- * Stack Overflow is for questions about programming. -->
* Stack Overflow는 프로그래밍에 관한 질문들을 올리는 사이트입니다.

<!-- * Server Fault is for questions about server and network administration. -->
* Server Fault는 서버와 네트워크 관리에 관련된 질문을 하는 사이트입니다.

<!-- Several projects have their own specific sites, including Android, Ubuntu, TeX/LaTeX, and SharePoint. Check the Stack Exchange site for an up-to-date list. -->
Android, Ubuntu, TeX/LaTeX, SharePoint 등 여러 프로젝트는 자기들만의 사이트를 Stack Exchange 안에 가지고 있는 경우가 있습니다. Stack Exchange 사이트에서 최신 목록을 확인하세요.

<div id='usefora'/>


### 웹 및 IRC 포럼

(*역주 : Internet Relay Chat(IRC) 는 단체 메신저 (카톡,Slack 등) 으로 생각하면 됩니다.*)

<!-- Your local user group, or your Linux distribution, may advertise a Web forum or IRC channel where newbies can get help. (In non-English-speaking countries newbie forums are still more likely to be mailing lists.) These are good first places to ask, especially if you think you may have tripped over a relatively simple or common problem. An advertised IRC channel is an open invitation to ask questions there and often get answers in real time. -->
당신이 속해있는 사용자 그룹, 또는 당신이 사용하는 리눅스 버전을 배포하는 그룹에서는 입문자들이 도움을 받을 수 있는 웹 포럼이나 채팅방을 종종 소개할 수 있습니다. (영어를 사용하지 않는 나라들에서는 뉴비들을 위한 포럼들이 아직도 메일링 리스트로 운영될 수 있습니다) 이런 포럼들이나 채팅방은 무언가 물어보기에 좋은 곳 중 하나입니다. 특히 당신이 상대적으로 쉬운 문제나 흔히 겪는 문제로 고생하고 있다면, 특히 좋을 겁니다. 홍보되는 채팅방은 누구나 질문을 할 수 있으며, 종종 실시간으로 답변을 받을 수도 있습니다.

<!-- In fact, if you got the program that is giving you problems from a Linux distribution (as is common today), it may be better to ask in the distro's forum/list before trying the program's project forum/list. The project's hackers may just say, “use _our_ build”. -->
특정 Linux distribution에서만 문제가 있는 프로그램을 쓰고 있다면(요즘에는 흔한 일입니다.) 원래 프로젝트의 포럼보다 해당 distro의 포럼에 먼저 물어보는 게 나을 수 있습니다. 원래 프로젝트의 해커들은 그냥 "*우리들이 직접 만든* 빌드를 쓰세요."라고 말하고 넘어갈 수 있습니다.

<!-- Before posting to any Web forum, check if it has a Search feature. If it does, try a couple of keyword searches for something like your problem; it just might help. If you did a general Web search before (as you should have), search the forum anyway; your Web-wide search engine might not have all of this forum indexed recently. -->
어떤 웹 포럼이던지 글을 쓰기 전에 검색 기능이 있는지 확인하세요. 검색 기능이 있다면, 당신의 문제와 관련이 있을 것 같은 키워드로 몇 번 검색을 시도해 보세요. 혹시라도 도움이 될 수도 있습니다. 당신이 일반적인 웹 검색을 이전에 했다면 (당연히 미리 해야 했지만), 그래도 포럼에서 검색을 해보세요. 당신이 사용한 검색 엔진이 포럼에서 최근에 올라온 글을  아직 등록하지 않았을 수 있습니다.

<!-- There is an increasing tendency for projects to do user support over a Web forum or IRC channel, with e-mail reserved more for development traffic. So look for those channels first when seeking project-specific help. -->
사용자 지원을 위해서 웹 포럼이나 채팅방을 사용하는 추세가 증가하고 있습니다. 이는 이메일을 개발에 직접적으로 관련된 이야기를 하기 위해 미리 남겨놓기 위함입니다. 그러니까 프로젝트와 직접적으로 관련된 문제에 대한 도움을 받기 위해서는 웹 포럼이나 채팅방을 먼저 찾아보세요.

<!-- In IRC, it's probably best not to dump a long problem description on the channel first thing; some people interpret this as channel-flooding. Best to utter a one-line problem description in a way pitched to start a conversation on the channel. -->
채팅방에서 질문을 할 때는, 문제에 대한 긴 설명을 채팅창에 바로 쏟아내는 건 좋지 못한 생각입니다. 어떤 사람들은 이런 행동을 채팅창을 도배한다고 받아들일 수 있습니다. 겪고 있는 문제에 대해 한 줄짜리 요약을 먼저 얘기하면서 대화를 시작하려고 해보세요.

<div id='uselists'/>

### 프로젝트 메일링 리스트는 차선책으로

<!-- When a project has a development mailing list, write to the mailing list, not to individual developers, even if you believe you know who can best answer your question. Check the documentation of the project and its homepage for the address of a project mailing list, and use it. There are several good reasons for this policy: -->
프로젝트에 개발진 메일링 리스트가 있다면, 개발자 개인에게 메일을 보내지 말고 메일링 리스트에 있는 사람들에게 보내세요. 설령 당신의 질문에 가장 잘 대답을 할 수 있는 사람을 알고 있다고 생각 하더라도요. 프로젝트 홈페이지에서 공식문서를 읽고 메일링 리스트를 찾아서 사용하세요. 이렇게 하는 것은 몇 가지 장점들이 있습니다:

<!-- * Any question good enough to be asked of one developer will also be of value to the whole group. Contrariwise, if you suspect your question is too dumb for a mailing list, it's not an excuse to harass individual developers. -->
* 어떤 개발진 인원에게 물어봐야 할 정도로 좋은 질문이라면 전체 개발진 및 사용자 그룹에도 도움이 될겁니다. 반대로, 당신의 질문이 메일링 리스트로 질문을 하기에 너무 멍청한 질문이라면 개발진들을 괴롭히게 되며, 메일링 리스트를 사용했더라도 변명의 여지가 없습니다.

<!-- * Asking questions on the list distributes load among developers. The individual developer (especially if he's the project leader) may be too busy to answer your questions. -->
* 메일링 리스트를 통해 질문을 하는 것은 개발진 개인에게 걸리는 부하를 줄여줍니다. 개발진 개인 (특히 그 사람이 프로젝트 리더라면) 당신에게 답변을 주기에 너무 바쁠 수도 있습니다.

<!-- * Most mailing lists are archived and the archives are indexed by search engines. If you ask your question on-list and it is answered, a future querent could find your question and the answer on the Web instead of asking it again. -->
* 대부분의 메일링 리스트들은 아카이브로 저장되어서 검색 엔진으로 접근할 수 있습니다. 당신이 올린 답변이 질문을 받는다면, 미래에 다른 사람이 똑같은 질문을 다시 하는 대신에 당신의 질문을 찾아서 답변을 얻을 수 있습니다.

<!-- * If certain questions are seen to be asked often, developers can use that information to improve the documentation or the software itself to be less confusing. But if those questions are asked in private, nobody has the complete picture of what questions are asked most often. -->
* 만약 특정 질문들이 계속 들어오는 게 확인된다면, 개발진들이 이를 반영하여 공식 문서를 개선하고 덜 헷갈리도록 수정하거나, 소프트웨어 자체를 고칠 수 있습니다. 하지만 만약 이런 질문들이 사적으로만 접수된다면, 아무도 어떤 질문이 많이 들어오는지 알 수가 없어서 전체적인 흐름을 알 수가 없습니다.

<!-- If a project has both a “user” and a “developer” (or “hacker”) mailing list or Web forum, and you are not hacking on the code, ask in the “user” list/forum. Do not assume that you will be welcome on the developer list, where they're likely to experience your question as noise disrupting their developer traffic. -->
만약에 해당 프로젝트가 "사용자"와 "개발진" (또는 "해커") 메일링 리스트를 둘 다 가지고 있고, 당신이 소스 코드에 대해서 파고들고 있는 게 아니라면, "사용자" 목록/포럼에 질문을 하세요. 개발자 포럼에서 당신의 질문이 환영받겠다고 생각하지 마세요. 개발자들은 당신의 질문을 개발자들 간의 의사소통을 방해하는 소음으로 느낄 가능성이 매우 높습니다.

<!-- However, if you are _sure_ your question is non-trivial, and you get no answer in the “user” list/forum for several days, try the “developer” one. You would be well advised to lurk there for a few daysor at least review the last few days of archived messages, to learn the local folkways before posting (actually this is good advice on any private or semi-private list). -->
만약 당신의 질문이 전혀 사소하지 않다(non-trivial)는 생각이 확실히 드는데도 사용자 포럼에서 답변을 며칠 동안 받지를 못했다면, 그때는 "개발자" 포럼을 이용해 보세요. 글을 쓰기 전에, 해당 포럼에 며칠 동안 상주하면서 지켜보거나, 최소한 지난 며칠 간의 저장된 메시지들을 읽어보면서 해당 포럼에 상주하는 사람들을 파악하는 것을 권장합니다. (사실 이 조언은 어떤 사설 혹은 준 사설 포럼에서도 적용됩니다.)

<!-- If you cannot find a project's mailing list address, but only see the address of the maintainer of the project, go ahead and write to the maintainer. But even in that case, don't assume that the mailing list doesn't exist. Mention in your e-mail that you tried and could not find the appropriate mailing list. Also mention that you don't object to having your message forwarded to other people. (Many people believe that private e-mail should remain private, even if there is nothing secret in it. By allowing your message to be forwarded you give your correspondent a choice about how to handle your e-mail.) -->
프로젝트 메일링 리스트를 찾을 수가 없고 프로젝트 관리자의 메일 주소만 적혀있다면 관리자에게 메일을 써도 됩니다. 다만, 메일링 리스트가 존재하지 않는다고 미리 생각하지 마세요. 메일을 적을 때 당신이 메일링 리스트를 찾아봤지만, 나오는 게 없다는 것을 알려주세요. 추가로 당신의 메일이 다른 사람들에게 전달(forward)되어도 상관없다는 사실을 알려주세요. (많은 사람은 개인적인 이메일은 아무런 비밀이 없는 내용이라도 함부로 공개하면 안 된다고 생각합니다. 메일을 다른 사람에게 전달해도 된다는 것을 알림으로써 메일을 받은 사람이 당신의 메일을 어떻게 처리 해야 할지 적절한 선택을 할 수 있는 여지를 주게 됩니다.)

<div id='bespecific'/>

<!-- ### Use meaningful, specific subject headers -->
### 구체적인 의미가 있는 말머리를 달아주세요

<!-- On mailing lists, newsgroups or Web forums, the subject header is your golden opportunity to attract qualified experts' attention in around 50 characters or fewer. Don't waste it on babble like “Please help me” (let alone “PLEASE HELP ME!!!!”; messages with subjects like that get discarded by reflex). Don't try to impress us with the depth of your anguish; use the space for a super-concise problem description instead. -->
주제와 관련된 말머리를 적는 것은 메일링 리스트, 뉴스그룹, 웹 포럼 등에서 50자 이내로 실력 있는 전문가들의 관심을 받기 위한 가장 좋은 기회입니다. 그 기회를 “Please help me” 같은 말로 웅얼거리는 데 낭비하지 마세요 (그렇다고 “PLEASE HELP ME!!!!” 같이 쓰지는 마세요. 이런 메시지들은 반사적으로 거부감을 느끼게 됩니다.). 우리의 관심을 끌기 위해서 본인이 얼마나 힘든 상황에 있는지 얘기하지 마세요. 그 대신에 매우 명료하고 간단하게 정리된 문제 상황을 적으세요.

<!-- One good convention for subject headers, used by many tech support organizations, is “object - deviation”. The “object” part specifies what thing or group of things is having a problem, and the “deviation” part describes the deviation from expected behavior. -->
수많은 기술적 지원을 하는 단체들에서 관습적으로 사용되는 말머리를 다는 규칙이 있는데, 그것은 바로 "주제 - 벗어난 정도" (*"object-deviation"*)입니다. "주제"에는 구체적으로 문제를 겪고 있는 대상들이 들어갑니다. "벗어난 정도"에는 예상되는 행동으로부터 얼마나 상황이 어긋났는지 적습니다.

<!-- **Stupid:** -->
**멍청한 예시**  

<!-- HELP! Video doesn't work properly on my laptop! -->
도와주세요! 랩탑에서 영상이 안틀어져요 ㅠ

<!-- **Smart:** -->
**똑똑한 예시**

<!-- X.org 6.8.1 misshapen mouse cursor, Fooware MV1005 vid. chipset -->
X.org 프로그램 6.8.1 버전 마우스 커서 모양 오류, Fooware MV1005 vid. 칩셋.

<!-- **Smarter:** -->
**더 똑똑한 예시**

<!-- X.org 6.8.1 mouse cursor on Fooware MV1005 vid. chipset - is misshapen -->
Fooware MV1005 vid. 칩셋 환경, X.org 프로그램 6.8.1 버전 마우스 커서 모양 오류

<!-- The process of writing an “object-deviation” description will help you organize your thinking about the problem in more detail. What is affected? Just the mouse cursor or other graphics too? Is this specific to the X.org version of X? To version 6.8.1? Is this specific to Fooware video chipsets? To model MV1005? A hacker who sees the result can immediately understand what it is that you are having a problem with _and_ the problem you are having, at a glance. -->
"주제 - 벗어난 정도" 식으로 문제 상황을 적는것은 당신이 가진 문제 상황에 대한 생각을 정리하는데 도움이 됩니다. 이것 때문에 영향을 받은 다른 프로그램이 있나? 마우스 커서만 문제가 있나, 그래픽 전체적으로 문제가 있나? 6.8.1 버전에서만 발생하는 것인가? 이게 Fooware 칩셋들에서만 발생하는 문제인가? 아니면 특정 모델 MV1005에서만? 이런 생각들을 통해 정리된 질문을 전문가들이 본다면 당신이 문제를 겪고 있는 상황, 그리고 여러분이 진짜로 겪고 있는 구체적인 문제를 한눈에 알 수가 있습니다.

<!-- More generally, imagine looking at the index of an archive of questions, with just the subject lines showing. Make your subject line reflect your question well enough that the next person searching the archive with a question similar to yours will be able to follow the thread to an answer rather than posting the question again. -->
조금 더 일반적으로 이야기하자면, 질문 제목들이 한 줄씩 쭉 적혀있는 게시판을 생각해 보세요. 당신이 적는 질문 제목이 당신의 질문 사항을 제대로 반영해야 당신과 비슷한 질문을 가진 다른 사람이 게시판을 검색할 때 새로운 게시물을 또 올리지 않고 당신이 썼던 글을 통해 답변으로 이동할 수 있습니다.

<!-- If you ask a question in a reply, be sure to change the subject line to indicate that you're asking a question. A Subject line that looks like “Re: test” or “Re: new bug” is less likely to attract useful amounts of attention. Also, pare quotation of previous messages to the minimum consistent with cluing in new readers. -->
답글을 통해서 추가 질문을 남기는 경우에, 주제란에 질문을 하기 위해 적은 글이라는 것을 밝혀주세요. "Re: test" 또는 "Re: new bug" 같은 내용은 유의미한 수준의 관심을 얻기가 힘들 겁니다. 추가로, 글을 새로 읽는 사람들을 위해서 과거에 주고받았던 메시지 내용을 일정량 이상 적어주세요.

<!-- Do not simply hit reply to a list message in order to start an entirely new thread. This will limit your audience. Some mail readers, like mutt, allow the user to sort by thread and then hide messages in a thread by folding the thread. Folks who do that will never see your message. -->
새 스레드를 만들기 위해서는 무작정 회신 버튼을 누르면 안 됩니다. 이는 청중들의 수를 제한적으로 만듭니다. Mutt와 같은 메일 리더 프로그램들은 사용자가 스레드별로 정렬하고, 스레드를 접어서 메시지를 숨길 수 있도록 설정할 수 있습니다. 이 기능을 사용하는 사람들은 당신의 메시지를 영영 볼 수 없을 겁니다.

<!-- Changing the subject is not sufficient. Mutt, and probably other mail readers, looks at other information in the e-mail's headers to assign it to a thread, not the subject line. Instead start an entirely new e-mail. -->
새로운 주제를 만들 때, 기존 메일에서 주제만을 바꾸는 건 충분하지 않습니다. Mutt를 포함한 다른 메일 리더 프로그램들은 주제 문장이 아니라 메일의 말머리를 통해서 해당 스레드에 메일을 배정합니다. 완전히 새로운 메일을 적어서 주제를 분리하세요.

<!-- On Web forums the rules of good practice are slightly different, because messages are usually much more tightly bound to specific discussion threads and often invisible outside those threads. Changing the subject when asking a question in reply is not essential. Not all forums even allow separate subject lines on replies, and nearly nobody reads them when they do. However, asking a question in a reply is a dubious practice in itself, because it will only be seen by those who are watching this thread. So, unless you are sure you _want_ to ask only the people currently active in the thread, start a new one. -->
웹 포럼에서는 조금 다른 게, 메시지들이 특정한 스레드에 더 강하게 묶여있고 해당 스레드 밖에서는 내용을 바로보기 어려운 경우가 있습니다. 답글을 통해 질문을 남길 때 답글 제목을 통해 주제 문장을 바꾸지 않아도 됩니다. 대부분 포럼은 답글을 달 때 제목을 달도록 하지 않고, 제목을 달더라도 잘 읽지 않습니다. 답글을 통해 질문을 하는 것은 그 자체로 효과가 의심스러운 게, 해당 스레드를 보는 사람들에게만 질문 내용이 보이기 때문입니다. 따라서 *해당 스레드를 보는 사람들에게만* 질문을 하고 싶은 게 아니라면, 새 스레드를 파는 게 낫습니다.

<div id='easyreply'/>

### 답변을 달기 쉽게 질문하세요

<!-- Finishing your query with “Please send your reply to... ” makes it quite unlikely you will get an answer. If you can't be bothered to take even the few seconds required to set up a correct Reply-To header in your mail agent, we can't be bothered to take even a few seconds to think about your problem. If your mail program doesn't permit this, [get a better mail program](http://linuxmafia.com/faq/Mail/muas.html). If your operating system doesn't support any e-mail programs that permit this, get a better operating system. -->
당신의 질문을 "답변을 아래 주소로 보내주세요 ... " 와 같은 형태로 끝낸다면 당신은 답변받을 수 없습니다. 메일 에이전트 프로그램에 단 몇 초를 투자해서 "답변하기" 버튼을 제대로 만들 노력도 하지 않는다면, 우리는 당신의 문제에 대해서 단 몇 초도 생각하기 싫습니다. 당신의 메일 프로그램에 그런 기능이 없다면, 더 좋은 [프로그램](http://linuxmafia.com/faq/Mail/muas.html)을 쓰세요. 당신의 운영체제에서 해당 기능을 제공하는 메일 프로그램들을 실행할 수 없다면, 더 좋은 운영체제를 장만하세요.

<!-- In Web forums, asking for a reply by e-mail is outright rude, unless you believe the information may be sensitive (and somebody will, for some unknown reason, let you but not the whole forum know it). If you want an e-mail copy when somebody replies in the thread, request that the Web forum send it; this feature is supported almost everywhere under options like “watch this thread”, “send e-mail on answers”, etc. -->
웹 포럼에서 개인 메일로 답변을 달라는 것은 명백히 무례한 행동입니다. 민감한 사항에 대한 질문 (또는 알 수 없는 이유로 답변을 다는 사람이 당신에게는 알려줄 수 있지만, 전체 포럼은 모르게 해야 하는 내용) 이라면요. 누군가가 단 답변을 메일로도 받아보고 싶어지면, 웹 포럼에 요청하세요. 거의 모든 곳에서 "이 스레드를 보기", "답변이 달리면 이메일로 알림 받기" 등의 기능을 제공합니다.

<div id='writewell'/>

<!-- ### Write in clear, grammatical, correctly-spelled language -->
### 명료하게, 올바른 문법으로, 올바른 맞춤법으로

<!-- We've found by experience that people who are careless and sloppy writers are usually also careless and sloppy at thinking and coding (often enough to bet on, anyway). Answering questions for careless and sloppy thinkers is not rewarding; we'd rather spend our time elsewhere. -->
우리는 경험적으로 대충 엉성하게 글을 쓰는 사람들은 코딩도 대충 얼렁뚱땅하는 것을 관찰하였습니다. (내기를 해도 좋을 정도로 말이죠). 생각하지 않는 사람들에게 답변을 다는 것은 보람이 없습니다. 우리는 차라리 그 시간을 다른 데 쓸 겁니다.

<!-- So expressing your question clearly and well is important. If you can't be bothered to do that, we can't be bothered to pay attention. Spend the extra effort to polish your language. It doesn't have to be stiff or formal — in fact, hacker culture values informal, slangy and humorous language used with precision. But it has to _be_ precise; there has to be some indication that you're thinking and paying attention. -->
따라서 당신의 질문을 잘 정리하고 명료하게 표현하는 게 중요합니다. 당신이 그런 노력을 기울이기가 싫다면, 우리도 당신 질문에 관심을 가지기 싫습니다. 질문의 문장을 다듬는 데 공을 들이세요. 이는 딱딱한 공식적인 문체를 사용해야 한다는 의미는 아닙니다. 사실, 해커들의 문화는 비공식적이고 유머러스한 문체로 말하고자 하는 내용을 정확하게 말하는 것을 좋아합니다. 다만 내용이 *정확해야* 합니다. 당신이 문제에 대해 집중하고 생각을 한다는 것을 나타내는 흔적이 있어야 합니다.

<!-- Spell, punctuate, and capitalize correctly. Don't confuse “its” with “it's”, “loose” with “lose”, or “discrete” with “discreet”. Don't TYPE IN ALL CAPS; this is read as shouting and considered rude. (All-smalls is only slightly less annoying, as it's difficult to read. Alan Cox can get away with it, but you can't.) -->
철자를 정확히 사용하고, 문장 부호를 정확하게 사용하고, 대문자를 정확하게 사용하게요. "it's"를 "its"로, "loose"를 "lose"로 쓴다거나, "discrete"를 "discreet"으로 혼동하지 마세요. (역주: 한국어로는 되/돼 외/왜 안/않 등이 해당합니다. 예시: ~~외않되요~~ 왜 안돼요*)

<!-- More generally, if you write like a semi-literate boob you will very likely be ignored. So don't use instant-messaging shortcuts. Spelling "you" as "u" makes you look like a semi-literate boob to save two entire keystrokes. Worse: writing like a l33t script kiddie hax0r is the absolute kiss of death and guarantees you will receive nothing but stony silence (or, at best, a heaping helping of scorn and sarcasm) in return. -->
조금 더 일반적으로 말하자면, 제대로 읽기 쓰기를 배우지 못한 사람처럼 글을 쓰면 무시당할 확률이 높습니다. 따라서 개인 메시지(카톡 등)에서 쓸법한 줄임말을 쓰지 마세요. "you"를 "u"로 쓰면 버튼 두 번 더 누르기를 귀찮아서 줄여 쓰는 못 배워먹은 사람으로 보입니다. 더 안 좋은 경우도 있습니다. 단어의 일부를 숫자나 부호로 대체해서 암호처럼 쓰는 것(*역주: leet을 l33t로, zero를 zer0 같이 쓰는 것*)은 좋아 보일 거 같지만 실제로는 최악입니다(kiss of death). 해커 놀이를 하는 애새끼처럼 보이고, 싸한 무관심(최선의 경우에도 멸시나 조롱)을 받을 것을 보장할 수 있습니다.(*역주: 한국어로 따지면 [ㄴr는 ㄱr끔 눈물을흘린ㄷr...](https://namu.wiki/w/%EC%B1%84%EC%97%B0?from=%EB%82%98%EB%8A%94%20%EA%B0%80%EB%81%94%20%EB%88%88%EB%AC%BC%EC%9D%84%20%ED%9D%98%EB%A6%B0%EB%8B%A4#s-5) 같은 느낌.*)

<!-- If you are asking questions in a forum that does not use your native language, you will get a limited amount of slack for spelling and grammar errors — but no extra slack at all for laziness (and yes, we can usually spot that difference). Also, unless you know what your respondent's languages are, write in English. Busy hackers tend to simply flush questions in languages they don't understand, and English is the working language of the Internet. By writing in English you minimize your chances that your question will be discarded unread. -->
당신의 모국어를 사용하지 않는 포럼에서 질문을 하는 경우에는, 철자와 문법에 대해서 조금은 정상참작을 받을 수는 있습니다. 하지만 게으른 질문은 정상참작이 되지 않습니다. (진심으로, 우리는 그 차이를 구분할 수 있습니다) 질문을 받는 사람이 사용하는 언어를 알 수 없다면 영어로 쓰세요. 해커들은 자기들이 읽을 수 없는 언어로 적힌 질문들을 변기 물 내리듯 치워버릴 겁니다. 또한, 인터넷의 공용어는 영어입니다. 영어로 질문을 쓰는 게 당신의 질문이 읽히지 않고 버려지는 확률을 최소화하는 겁니다.

<!-- If you are writing in English but it is a second language for you, it is good form to alert potential respondents to potential language difficulties and options for getting around them. Examples: -->
당신이 영어로 글을 쓰는데 영어가 주 언어가 아니라면, 글을 보는 사람들에게 언어적인 문제가 있을 수 있다는 것을 알리고 도움을 받을 수 있는 선택지를 같이 적어주세요.  
예를 들자면:  
(*역주: 실제로 사용할 수 있는 문구들은 원문을 병기합니다.*)

<!-- * English is not my native language; please excuse typing errors. -->
* 영어가 제 모국어가 아니라서 오탈자가 있을 수 있습니다. 양해 부탁드립니다.(*원문 : English is not my native language; please excuse typing errors.*)

<!-- * If you speak $LANGUAGE, please email/PM me; I may need assistance translating my question. -->
* 당신이 $LANGUAGE 언어를 쓸 줄 안다면, 이메일이나 개인 메시지를 주세요. 질문을 번역하는데 도움이 필요할 수도 있습니다.(*원문: If you speak $LANGUAGE, please email/PM me; I may need assistance translating my question.*)

<!-- * I am familiar with the technical terms, but some slang expressions and idioms are difficult for me. -->
* 기술적인 용어들은 익숙하지만, 유행어나 속담, 숙어는 이해하기에 어렵습니다.

<!-- * I've posted my question in $LANGUAGE and English. I'll be glad to translate responses, if you only use one or the other. -->
* 질문을 $LANGUAGE 와 영어로 같이 적었습니다. 영어나 $LANGUAGE 로 질문을 옮기는데 도움을 주시면 감사하겠습니다.

<div id='formats'/>

<!-- ### Send questions in accessible, standard formats -->
### 질문을 접근성이 좋고, 표준적인 양식으로 작성하세요

<!-- If you make your question artificially hard to read, it is more likely to be passed over in favor of one that isn't. So: -->
당신이 질문을 의도적으로 읽기 힘들게 쓴다면, 그렇지 않은 질문들에 비해서 답변받기에 어렵겠죠.  
따라서 아래 방법들을 고려하세요:

<!-- * Send plain text mail, not HTML. (It's not hard to [turn off HTML](http://www.birdhouse.org/etc/evilmail.html).) -->
* HTML 대신 평문(plain text)으로 메일을 작성하세요. (HTML 기능을 끄는 것은 어렵지 않습니다. [링크](http://www.birdhouse.org/etc/evilmail.html))

<!-- * MIME attachments are usually OK, but only if they are real content (such as an attached source file or patch), and not merely boilerplate generated by your mail client (such as another copy of your message). -->
* 첨부 파일은 실질적인 내용이 있는 경우에는 대체적으로 괜찮습니다. (소스코드나 패치파일 등.) 메일 클라이언트가 의미 없이 자동으로 생성하는 파일은 안됩니다 (메일 내용의 사본 등).

<!-- * Don't send e-mail in which entire paragraphs are single multiply-wrapped lines. (This makes it too difficult to reply to just part of the message.) Assume that your respondents will be reading mail on 80-character-wide text displays and set your line wrap accordingly, to something less than 80. -->
* 줄 바꿈을 하지 않고 한 문단을 이어서 쓰는 건 금물입니다. (메시지의 부분만 집어서 답변하기 곤란합니다) 메일을 읽는 사람 디스플레이에 대략 80줄이 한 줄로 들어간다고 생각하고, 한 줄이 80자보다 적게 줄 바꿈을 하세요. (*역주 : single multiply-wrapped lines에 대한 번역입니다. 현재는 사장된 개념으로 추정됩니다.*)

<!-- * However, do _not_ wrap data (such as log file dumps or session transcripts) at any fixed column width. Data should be included as-is, so respondents can have confidence that they are seeing what you saw. -->
* 하지만 (로그 파일이나 세션 사본 같은) 데이터는 고정 열 너비 형태로 바꾸지 마세요. 데이터는 있는 그대로 보여야 하고, 읽는 사람이 당신이 본 것과 같은 것을 보고 있다는 확신을 가지도록 해야 합니다.

<!-- * Don't send MIME Quoted-Printable encoding to an English-language forum. This encoding can be necessary when you're posting in a language ASCII doesn't cover, but many e-mail agents don't support it. When they break, all those =20 glyphs scattered through the text are ugly and distracting — or may actively sabotage the semantics of your text. -->
* 영어를 사용하는 포럼에서 [MIME Quoted-Printable encoding](https://en.wikipedia.org/wiki/Quoted-printable)으로 내용은 적지를 마세요. 해당 encoding은 ASCII로 표현할 수 없는 언어들을 사용할 때는 필요하겠지만, 많은 이메일 시스템은 지원하지 않습니다. 해당 문자들이 깨진다면 '=20' 들이 본문에 가득해서 본문의 가독성을 해치고 읽을 수가 없을 정도이거나, 당신의 본문을 매우 능동적으로 망가뜨려 버립니다.

<!-- * Never, _ever_ expect hackers to be able to read closed proprietary document formats like Microsoft Word or Excel. Most hackers react to these about as well as you would to having a pile of steaming pig manure dumped on your doorstep. Even when they can cope, they resent having to do so. -->
* 절대로, *절대로* 해커들이 Microsoft Word 나 Excel같이 특정 프로그램이 있어야만 읽을 수 있는(closed proprietary document format) 문서 형식을 읽을 것으로 생각하지 마세요. 많은 해커는 그런 파일들을 마주할 때 누군가가 문 앞에다 돼지 분뇨를 쏟아놓고 간 것처럼 반응 할 겁니다. 그 힘든 걸 견뎌낼 수 있더라도, 그러지 않는 것을 선택 할 겁니다.

<!-- * If you're sending e-mail from a Windows machine, turn off Microsoft's problematic “Smart Quotes” feature (From Tools > AutoCorrect Options, clear the smart quotes checkbox under AutoFormat As You Type.). This is so you'll avoid sprinkling garbage characters through your mail. -->
* 당신이 Windows에서 이메일을 보낸다면, Microsoft 사의 문제가 많은 ["Smart Quotes"](https://support.microsoft.com/en-us/office/smart-quotes-in-word-702fc92e-b723-4e3d-b2cc-71dedaf2f343) 기능을 꺼야 합니다. (Tools > AutoCorrect Options > AutoFormat As You Type 에서 끌 수 있습니다) 이렇게 해야 메일 본문에 쓰레기 문자들이 흩뿌려지는 상황을 방지할 수 있습니다.

<!-- * In Web forums, do not abuse “smiley” and “HTML” features (when they are present). A smiley or two is usually OK, but colored fancy text tends to make people think you are lame. Seriously overusing smileys and color and fonts will make you come off like a giggly teenage girl, which is not generally a good idea unless you are more interested in sex than answers. -->
웹 포럼에서 ["smiley"](https://en.wikipedia.org/wiki/Smiley) (*역주: 요즘 시대로 따지면 emoji*)나 "HTML" 기능들을 남발하지 마세요 (해당 포럼이 기능을 지원한다면 말이죠). 한두 개는 괜찮을 수도 있는데, 알록달록한 컬러 텍스트를 사용한다면 사람들이 병신같이 볼 겁니다. Smiley, 요란한 색깔과 글씨체 등을 본문에 남발하는 건 떨어지는 낙엽만 봐도 웃을 나이의 청소년 여자아이처럼 보일 겁니다. 답변을 얻는 것보다 섹스에 관심이 있는 게 아니라면 일반적으로 좋은 생각이 아닙니다.

<!-- If you're using a graphical-user-interface mail client such as Netscape Messenger, MS Outlook, or their ilk, beware that it may violate these rules when used with its default settings. Most such clients have a menu-based “View Source” command. Use this on something in your sent-mail folder, verifying sending of plain text without unnecessary attached crud. -->
당신이 Netscape Messenger, MS Outlook, 혹은 이와 유사한 GUI 이메일 클라이언트를 사용한다면 해당 프로그램이 위 규칙들을 어기는 설정이 기본으로 되어있을 수도 있습니다. 대부분 클라이언트 들은 "소스 보기(View Source)" 기능을 지원합니다. 보낸 메일함에서 해당 기능을 통해 평문이 잘 적혀있고 불필요한 문자열들이 포함되지는 않았는지 확인하세요.

<div id='beprecise'/>

<!-- ### Be precise and informative about your problem -->
### 문제에 대해서 구체적이고 정확하게 서술하세요

<!-- * Describe the symptoms of your problem or bug carefully and clearly. -->
* 겪고있는 문제나 버그의 증상을 명료하고 주의깊게 설명하세요.

<!-- * Describe the environment in which it occurs (machine, OS, application, whatever). Provide your vendor's distribution and release level (e.g.: “Fedora Core 7”, “Slackware 9.1”, etc.). -->
* 어떤 환경에서 발생하는 문제인지 알려주세요 (기종, OS, 앱 등). 어떤 버전/릴리스 인지도 알려주세요 (e.g.: "Fedora Core 7", "Slackware 9.1" 등).

<!-- * Describe the research you did to try and understand the problem before you asked the question. -->
* 질문글을 올리기 전에 문제 상황을 파악하기 위해서 어떤 시도들을 해봤는지 설명하세요.

<!-- * Describe the diagnostic steps you took to try and pin down the problem yourself before you asked the question. -->
* 질문글을 올리기 전에 문제의 범위를 좁혀서 구체적으로 파악하기 위해서 택했던 진단 방법을 설명하세요.

<!-- * Describe any possibly relevant recent changes in your computer or software configuration. -->
* 최근 컴퓨터나 SW 설정에 변화가 있었던 경우, 관련이 있을 수 있는 변화 내용을 적어주세요.

<!-- * If at all possible, provide a way to _reproduce the problem in a controlled environment_. -->
* 가능하다면, *변인 통제가 된 상태에서 문제 상황을 재현 할 수 있는 방법*을 알려주세요.

<!-- Do the best you can to anticipate the questions a hacker will ask, and answer them in advance in your request for help. -->
해커들이 물어볼 것 같은 내용들을 최대한 예상해서 사전에 해당 내용에 대한 설명을 도움을 요청할 때 같이 적으세요.  

<!-- Giving hackers the ability to reproduce the problem in a controlled environment is especially important if you are reporting something you think is a bug in code. When you do this, your odds of getting a useful answer and the speed with which you are likely to get that answer both improve tremendously. -->
코드에 버그가 있다고 생각하여 이를 알리려고 할 때, 해커들이 변인 통제가 된 환경에서 문제를 재현할 수 있도록 하는것은 매우 중요합니다.
당신이 문제를 재현 가능하게 도와준다면, 유용한 답변을 받을 확률과 답변을 받는 속도가 어마어마하게 커집니다.

<!-- Simon Tatham has written an excellent essay entitled [How to Report Bugs Effectively](http://www.chiark.greenend.org.uk/~sgtatham/bugs.html). I strongly recommend that you read it. -->
Simon Tatham 은 [효과적으로 버그를 알리는 법 How to Report Bugs Effectively](http://www.chiark.greenend.org.uk/~sgtatham/bugs.html) 에 관해서 아주 훌륭한 글을 쓴 적이 있습니다. 이 글을 읽어보는 것을 강력하게 추천합니다.

<div id='volume'/>

<!-- ### Volume is not precision -->
### 양 보다는 질

<!-- You need to be precise and informative. This end is not served by simply dumping huge volumes of code or data into a help request. If you have a large, complicated test case that is breaking a program, try to trim it and make it as small as possible. -->
당신은 정확하고 정보성이 있도록 질문글을 써야합니다. 이는 단순히 많은 양의 코드와 데이터를 도움을 요청할 때 싸지르는걸 의미하지 않습니다.
만약 프로그램을 망가뜨리는 크고 복잡한 테스트 케이스가 있다면, 최대한 작게 줄여야 합니다.

<!-- This is useful for at least three reasons. One: being seen to invest effort in simplifying the question makes it more likely you'll get an answer, Two: simplifying the question makes it more likely you'll get a _useful_ answer. Three: In the process of refining your bug report, you may develop a fix or workaround yourself. -->
이는 세 가지 이유로 효과적입니다. 첫 번째로, 질문을 간결하게 하려는 시도가 보인다면 답변을 받을 확률이 높아집니다. 두 번째로, 질문을 간결하게 하는것은 *쓸모있는* 답변을 받을 확률을 높여줍니다. 세 번째로, 작성한 버그 리포트를 다듬는 과정에서 본인 스스로 버그를 고칠 수 있거나 버그가 생기는 상황을 피해가는 방법을 만들 수 있습니다.

<div id='idm368'/>

<!-- ### Don't rush to claim that you have found a bug -->
### 섣불리 버그를 발견했다고 결론내리지 마세요

<!-- When you are having problems with a piece of software, don't claim you have found a bug unless you are very, _very_ sure of your ground. Hint: unless you can provide a source-code patch that fixes the problem, or a regression test against a previous version that demonstrates incorrect behavior, you are probably not sure enough. This applies to webpages and documentation, too; if you have found a documentation “bug”, you should supply replacement text and which pages it should go on. -->
특정 소프트웨어로 인해서 문제를 겪고 있을 때, 아주 *아주* 확실한 근거가 없는 한 버그를 찾았다고 주장하지 마세요. 어떻게 아는지 힌트를 드리자면: 문제를 해결하는 소스 코드 패치를 제공할 수 있거나, 이전 버전과 대비해서 정확하지 않게 동작하는 부분을 정확히 밝혀내는 회귀 테스트를 한 경우가 아니라면 당신은 확실하지 않은 겁니다. 이는 웹페이지와 공식 문서에도 적용됩니다. 당신이 만약 공식 문서에 잘못된 "버그"가 있다고 이야기한다면, 당신은 몇 페이지 어디의 내용이 바뀌어야 하는지와 어떻게 고쳐야 할지 내용을 제시해야 합니다.

<!-- Remember, there are many other users that are not experiencing your problem. Otherwise you would have learned about it while reading the documentation and searching the Web (you did do that before complaining, [didn't you](#질문을-하기에-앞서서 "Before You Ask")?). This means that very probably it is you who are doing something wrong, not the software. -->
당신과 같은 문제를 겪지 않는 사용자들이 매무 많다는 것을 명심하세요. 당신과 같은 문제를 겪는 사람들이 많은 경우에는 공식 문서를 읽거나 웹 검색을 통해서 진작에 답을 찾을 수 있었을겁니다 (불평불만 하기 전에 [찾아보기는 했겠죠? ^^](#질문을-하기에-앞서서))

<!-- The people who wrote the software work very hard to make it work as well as possible. If you claim you have found a bug, you'll be impugning their competence, which may offend some of them even if you are correct. It's especially undiplomatic to yell “bug” in the Subject line. -->
소프트웨어를 작성 한 사람들은 최대한 그것이 잘 작동하도록 만들기 위해서 심혈을 기울입니다. 당신이 버그를 찾았다고 주장을 하는 것은, 그것은 작성을 한 사람의 능력을 의심하게 만드는 것이고, 개 중 일부는 당신이 설령 맞는다고 하더라도 불쾌하게 받아들일 수도 있습니다. 특히 주제 제목에다가 "버그래요" 라고 소리 지르고 다니는 것은 눈치가 없는 행동입니다.

<!-- When asking your question, it is best to write as though you assume _you_ are doing something wrong, even if you are privately pretty sure you have found an actual bug. If there really is a bug, you will hear about it in the answer. Play it so the maintainers will want to apologize to you if the bug is real, rather than so that you will owe them an apology if you have messed up. -->
질문을 할 때, *당신 본인이* 뭔가를 잘못하고 있다는 것처럼 이야기하는 것이 상책입니다. 당신이 개인적으로 실제 있는 버그를 찾았다고 확신하더라도 말이죠. 만약에 진짜 버그였다면, 당신은 답변을 통해 알 수 있을 겁니다. 프로젝트 관리자들이 버그가 있어서 미안하다고 말하도록 만드는 것이, 질문자 본인이 버그가 있었음에도 미안하다는 말을 해야 하는 상황보다는 나을 겁니다.

<div id='idm379'/>

<!-- ### Grovelling is not a substitute for doing your homework -->
### 굽신거린다고 당신이 해야하는 일이 면제되지는 않습니다

<!-- Some people who get that they shouldn't behave rudely or arrogantly, demanding an answer, retreat to the opposite extreme of grovelling. “I know I'm just a pathetic newbie loser, but...”. This is distracting and unhelpful. It's especially annoying when it's coupled with vagueness about the actual problem. -->
건방지거나 무례한 태도, 답변을 요구하는 태도로 질문을 하면 안 된다는 사실을 이해하는 사람 중 일부는 완전히 반대 방향으로 빠져버려서 극단적으로 굽신거리게 됩니다. "저도 제가 병신같고 한심한 뉴비인걸아는데..." 같은 식으로 말이죠. 이는 본질을 호도하며 쓸모도 없는 말 입니다. 이는 특히 불분명한 문제 상황 묘사와 함께 쓰이는 경우 굉장히 열받습니다.

<!-- Don't waste your time, or ours, on crude primate politics. Instead, present the background facts and your question as clearly as you can. That is a better way to position yourself than by grovelling. -->
당신이 해야 할 일을 남에게 떠넘기기 위해서 원숭이들도 알아챌 얕은수를 쓰느라 당신의 시간을 낭비하지도 말고, 우리의 시간을 낭비하지도 마세요. 대신에 질문의 배경에 관련된 사실을 충실히 쓰고 당신의 질문을 할 수 있는 한 명료하게 쓰세요. 그렇게 하는 게 굽신거리는 것보다 훨씬 나은 방법입니다.

<!-- Sometimes Web forums have separate places for newbie questions. If you feel you do have a newbie question, just go there. But don't grovel there either. -->
가끔 웹 포럼들은 초보적인 질문을 위한 공간을 따로 분리하는 경우가 있습니다. 당신이 초보적인 질문거리를 가지고 있다고 느낀다면, 그냥 거기로 가시면 됩니다. 거기 가서도 굽신거릴 필요는 전혀 없고요.

<div id = 'symptoms'/>

<!-- ### Describe the problem's symptoms, not your guesses -->
### 당신의 뇌피셜 대신 문제 증상을 설명하세요

<!-- It's not useful to tell hackers what you think is causing your problem. (If your diagnostic theories were such hot stuff, would you be consulting others for help?) So, make sure you're telling them the raw symptoms of what goes wrong, rather than your interpretations and theories. Let them do the interpretation and diagnosis. If you feel it's important to state your guess, clearly label it as such and describe why that answer isn't working for you. -->
해커들에게 당신이 생각하기에 뭐가 문제인지 얘기를 하는 건 딱히 쓸모가 없습니다. (당신이 가진 문제 진단에 대한 생각이 그렇게 대단하다면, 다른 사람들에게 물어보러 다니고 있을까요?) 그러니까 당신이 문제를 어떻게 해석하는지, 문제에 대해서 어떻게 생각하는지 얘기를 하지 말고 있는 그대로 발생하는 문제 증상을 얘기하도록 하세요. 당신 생각을 얘기하는 게 중요하다고 생각되는 경우라면, 당신의 주관적인 생각임을 확실히 밝히고 해결법들이 당신에게는 통하지 않는 이유를 구체적으로 적으세요.

<!-- **Stupid:** -->
**병신같은 사례:**

<!-- I'm getting back-to-back SIG11 errors on kernel compiles, and suspect a hairline crack on one of the motherboard traces. What's the best way to check for those? -->
커널을 컴파일할 때마다 연속으로 SIG11 오류가 발생하고 있는데, 마더보드 기록에 아주 미세한 오류가 있는 것 같습니다. 이런 문제를 확인하려면 어떻게 해야 하나요?

<!-- **Smart:** -->
**올바른 사례:**

<!-- My home-built K6/233 on an FIC-PA2007 motherboard (VIA Apollo VP2 chipset) with 256MB Corsair PC133 SDRAM starts getting frequent SIG11 errors about 20 minutes after power-on during the course of kernel compiles, but never in the first 20 minutes. Rebooting doesn't restart the clock, but powering down overnight does. Swapping out all RAM didn't help. The relevant part of a typical compile session log follows. -->
제가 직접 조립한 K6/233시스템은 FIC-PA2007(VIA Apollo VP2 칩셋) 마더보드, 256MB Corsair PC133 SDRAM을 추가하여 구성하였는데요,
전원을 켜고 커널 컴파일이 시작된 이후 20분 뒤에 SIG11 오류를 겪는 것이 반복되고 있습니다. 특이할 점은, 처음 20분 동안에는 문제를 겪은 적이 한 번도 없습니다. 재부팅을 해도 컴퓨터 클락이 초기화가 되지 않으며, 밤새 전원을 꺼둬야 초기화가 됩니다. 메모리 스왑을 해도 해결이 되지 않습니다. 컴파일 세션 동안 작성되는 로그 파일 중 관련 있는 일부를 다음과 같이 첨부합니다.

<!-- Since the preceding point seems to be a tough one for many people to grasp, here's a phrase to remind you: "All diagnosticians are from Missouri." That US state's official motto is "Show me" (earned in 1899, when Congressman Willard D. Vandiver said "I come from a country that raises corn and cotton and cockleburs and Democrats, and frothy eloquence neither convinces nor satisfies me. I'm from Missouri. You've got to show me.") In diagnosticians' case, it's not a matter of skepticism, but rather a literal, functional need to see whatever is as close as possible to the same raw evidence that you see, rather than your surmises and summaries. Show us. -->
앞의 예시가 많은 사람에게 이해하기 어려울 수도 있다는 생각이 들어서, 떠올리면 좋은 격언 하나를 소개합니다. "모든 분석가는 미주리에서 왔다." 미주리주의 공식 표어는 "보여주지 않으면 믿을 수 없다."이기 때문이죠. (1899년 미국 하원의원 Willard D. Vandiver가 "나는 옥수수와 솜, 우엉, 그리고 민주당을 키우는 동네에서 왔고, 허황되고 실속이 없는 연설은 나는 믿을 수도 없고, 만족할 수도 없다. 나는 미주리에서 왔다. 네가 가진걸 보여주지 않으면 나는 믿지 않겠다.") 분석하고 진단을 하는 사람들 입장에서 이는 회의론적인 문제가 아니라, 진짜 문자 그대로 의미이기도 합니다. 또한 기능적인 의미도 있는데, 당신의 추정과 요약을 거치치 않은, 가공되지 않은 생생한 증거를 뭐라도 보여줘야 판단을 할 수 있기 때문입니다. 우리에게 증거를 보여주세요. (*역주: 요점은 "너 생각은 중요하지 않으니, 문제 상황을 있는 그대로 설명해라" 입니다.*)

<div id='chronology'/>

<!-- ### Describe your problem's symptoms in chronological order -->
### 문제 증상들을 시간 순서대로 나열하세요

<!-- The clues most useful in figuring out something that went wrong often lie in the events immediately prior. So, your account should describe precisely what you did, and what the machine and software did, leading up to the blowup. In the case of command-line processes, having a session log (e.g., using the script utility) and quoting the relevant twenty or so lines is very useful. -->
무엇이 잘못되었는지 파악하는 데 있어서 가장 쓸모 있는 단서들은 보통 잘못되기 직전에 무슨 일이 일어났는지 파악하는 데서 얻을 수 있습니다. 그러므로, 당신은 정확히 당신이 한 행동들을 설명해야 하고, 그 행동으로 인해서 컴퓨터와 소프트웨어가 어떻게 동작했는지를 터지게 되었던 시점까지 채워야 합니다. 커맨드라인을 사용하는 과정인 경우 세션 로그(예를 들어 script utility 같은 것)를 확보하고 관련된 20여 줄을 첨부하는 건 매우 도움이 됩니다.

<!-- If the program that blew up on you has diagnostic options (such as -v for verbose), try to select options that will add useful debugging information to the transcript. Remember that more is not necessarily better; try to choose a debug level that will inform rather than drowning the reader in junk. -->
터뜨린 프로그램에 문제 진단과 관련된 옵션이 있다면(-v를 통한 verbose 옵션 등), 해당 진단 옵션들을 사용하여 디버깅에 유용한 정보들이 표시되도록 만들 수 있습니다. 주의할 점은 양보다는 질이라는 겁니다. 적절한 양의 디버그 옵션을 선택해서 읽는 사람들이 너무 많은 양의 정보를 허우적거리다가 익사하지 않도록 해야 합니다.

<!-- If your account ends up being long (more than about four paragraphs), it might be useful to succinctly state the problem up top, then follow with the chronological tale. That way, hackers will know what to watch for in reading your account. -->
증상 설명이 너무 길어지는 경우(4문단 이상), 문제점을 간결하게 맨 위에 적어놓고 밑에다 시간순으로 이야기를 나열하는 것도 좋습니다. 그렇게 하면, 해커들이 아래 내용을 읽는 동안 무엇을 봐야 하는지 알 수 있기 때문입니다.

<div id='goal'/>

<!-- ### Describe the goal, not the step -->
### 과정을 이야기 하지 말고, 목표를 얘기하세요

<!-- If you are trying to find out how to do something (as opposed to reporting a bug), begin by describing the goal. Only then describe the particular step towards it that you are blocked on. -->
상황을 해결하기 위한 방법을 찾는 중이라면 (버그를 신고하는 것과 반대로) 무엇을 하고자 하는 목표부터 설명하는 것이 좋습니다. 그러고 나서 당신이 막혀있는 지점에 도달하게 되는 과정을 설명하세요.

<!-- Often, people who need technical help have a high-level goal in mind and get stuck on what they think is one particular path towards the goal. They come for help with the step, but don't realize that the path is wrong. It can take substantial effort to get past this. -->
기술적인 도움이 필요한 사람들은 자신이 가진 개념적인 목표를 달성하기 위해 단 하나의 방법이 있다고 믿어서 막혀있는 경우가 종종 있습니다. 그 사람들은 그 방법으로 가는 중에 맞닥뜨리는 특정한 단계에서만 도움을 받으려고 하는데, 애초에 그 방법 자체가 잘못되었다는 사실을 인지하지 못하는 경우가 있습니다. 이런 경우에는 빠져나오는 게 상당히 힘듭니다.

<!-- **Stupid:** -->
**병신같은 질문**

<!-- How do I get the color-picker on the FooDraw program to take a hexadecimal RGB value? -->
FooDraw 프로그램에서 RGB hex 값을 보기 위한 color-picker를 어떻게 구할 수 있나요?

<!-- **Smart:** -->
**똑똑한 질문**

<!-- I'm trying to replace the color table on an image with values of my choosing. Right now the only way I can see to do this is by editing each table slot, but I can't get FooDraw's color picker to take a hexadecimal RGB value. -->
내 선택에 따라서 내가 원하는 대로 이미지의 컬러 테이블을 바꿀 수 있는 방법을 찾고 있습니다. 지금 제가 하는 방법은 각 컬러 테이블 칸을 하나씩 바꾸는 것밖에 없는데요, Foo Draw 의 color picker는 RGB 값의 hex 값을 볼 수가 없어서 문제입니다.

<!-- The second version of the question is smart. It allows an answer that suggests a tool better suited to the task. -->
두 번째 버전의 질문은 꽤 똑똑한 질문입니다. 해당 작업을 하는데 더 적합한 도구를 추천할 수 있도록 하기 때문입니다.

<div id='noprivate'/>

<!-- ### Don't ask people to reply by private e-mail -->
### 개인 이메일로 답변을 달라고 요구하지 마세요

<!-- Hackers believe solving problems should be a public, transparent process during which a first try at an answer can and should be corrected if someone more knowledgeable notices that it is incomplete or incorrect. Also, helpers get some of their reward for being respondents from being seen to be competent and knowledgeable by their peers. -->
해커들은 문제를 해결하는 것은 투명하게 공개된 방법으로 진행되어야 한다고 믿습니다. 이는 처음에 달린 답변이 완전하지 않거나 잘못된 답변인 경우, 더 잘 알고 있는 사람이 고칠 수 있어야 하며 고쳐져야 하기 때문입니다. 또한, 도움을 주는 사람들은 자기 주변의 사람으로부터 능력이 있다는 것을 인정받음으로써 답변을 달면서 얻는 즐거움 중 일부를 얻을 수 있습니다.

<!-- When you ask for a private reply, you are disrupting both the process and the reward. Don't do this. It's the _respondent's_ choice whether to reply privately — and if he or she does, it's usually because he or she thinks the question is too ill-formed or obvious to be interesting to others. -->
개인적으로 답변을 요청하는 건 답변하는 과정과 답변을 함으로써 얻는 보람 두 가지에 모두 해를 끼치는 방법입니다. 하지 마세요. *답변을 다는 사람이* 개인적으로 답변을 할지 결정하는 겁니다. 또한 개인적으로 답변을 한다는 경우는 답변한다는 사람이 느끼기에 질문이 너무 잘못 쓰여 있거나 너무 당연한 질문이라서 답변을 달 가치가 별로 없는 경우가 다반사입니다.

<!-- There is one limited exception to this rule. If you think the question is such that you are likely to get many answers that are all closely similar, then the magic words are “e-mail me and I'll summarize the answers for the group”. It is courteous to try and save the mailing list or newsgroup a flood of substantially identical postings — but you have to keep the promise to summarize. -->
예외적인 경우가 딱 한 가지, 제한적으로 있습니다. 질문에 대하여 중복되는 답변을 많이 받을 가능성이 높다고 판단되는 경우, "개인적인 이메일로 답변을 주시면 답변을 요약해서 뉴스그룹에 다시 올리겠습니다."라는 마법의 문장을 사용할 수 있습니다. 이런 식으로 메일링 리스트나 뉴스그룹이 중복된 내용으로 범람 되는 것을 막는 것은 굉장히 바람직한 행동입니다. 다만, 요약해서 다시 올리겠다는 약속은 지켜야겠죠. (*역주: 뉴스그룹과 메일링 리스트가 2023년 현재로서는 deprecated 되었기에 더 이상 유효한 방법은 아닙니다.*)

<div id='explicit'/>

<!-- ### Be explicit about your question -->
### 질문을 명확하게 하세요

<!-- Open-ended questions tend to be perceived as open-ended time sinks. Those people most likely to be able to give you a useful answer are also the busiest people (if only because they take on the most work themselves). People like that are allergic to open-ended time sinks, thus they tend to be allergic to open-ended questions. -->
열린 질문은 끝없이 시간을 빨아먹는 기계로 받아들여지기 일쑤입니다. (*역주: 열린 질문은 예, 아니오로 답변할 수 없는 질문을 의미합니다. 열린 질문: 좋아하는 커피 있어? / 닫힌 질문: 아인슈페너 좋아하니?) 당신에게 유용한 답변을 줄 수 있는 확률이 가장 높은 사람은 동시에 가장 바쁜 사람이기도 합니다. (그 사람들이 대부분의 일을 맡고 있기 때문이지요.) 이런 사람들은 기약 없이 시간을 빨아먹는 행동들에 신경질을 내며, 따라서 열린 질문에도 신경질적 반응을 보입니다.

<!-- You are more likely to get a useful response if you are explicit about what you want respondents to do (provide pointers, send code, check your patch, whatever). This will focus their effort and implicitly put an upper bound on the time and energy a respondent must allocate to helping you. This is good. -->
질문을 답변하려는 사람에게서 받고자 하는 도움을 명확하게 적는 것이 유용한 답변을 얻을 확률을 높여줍니다. (어떤 자료를 참조하도록 알려줘야 하는지, 코드를 봐줘야 하는지, 패치를 체크해야 하는지 등입니다) 이는 답변하는 사람이 당신을 도와주기 위해서 들여야 하는 시간과 노력의 상한선을 어느 정도 가늠하는 데 도움을 주고 당신을 도와주는데 노력을 집중시킬 수 있습니다. 이는 바람직한 현상입니다.

<!-- To understand the world the experts live in, think of expertise as an abundant resource and time to respond as a scarce one. The less of a time commitment you implicitly ask for, the more likely you are to get an answer from someone really good and really busy. -->
전문가들이 살아가는 세계에 대해서 이해를 돕자면, 능력은 풍족하고 시간은 쪼들리는 상황이라고 생각하면 됩니다. 도와주는 데 필요한 시간을 줄여서 부탁할수록, 정말 바쁘고 능력 있는 사람에게서 답변받을 확률이 높아집니다.

<!-- So it is useful to frame your question to minimize the time commitment required for an expert to field it — but this is often not the same thing as simplifying the question. Thus, for example, “Would you give me a pointer to a good explanation of X?” is usually a smarter question than “Would you explain X, please?”. If you have some malfunctioning code, it is usually smarter to ask for someone to explain what's wrong with it than it is to ask someone to fix it. -->
따라서 전문가들이 당신의 질문을 답변하는 데 필요한 노력을 줄이는 방향으로 질문의 가닥을 잡는 게 도움이 됩니다. 다만, 이는 질문을 단순화하는 것과 같지는 않습니다. 예를 들어서, "X에 대한 안내가 잘 되어있는 참조 자료를 주실 수 있나요?"라는 질문은 "X를 설명 좀 해주세요."라는 질문보다 대부분의 상황에서 더 똑똑한 질문입니다. 당신이 제대로 동작하지 않는 코드로 문제를 겪고 있다면, 무엇이 잘못되었는지 알려달라고 요청하는 게 잘못된 부분을 고쳐 달라고 하는 것 보다 대부분의 경우에서 더 똑똑한 질문입니다.

<div id='code'/>

<!-- ### When asking about code -->
### 코드에 대해 질문을 할 때

<!-- Don't ask others to debug your broken code without giving a hint what sort of problem they should be searching for. Posting a few hundred lines of code, saying "it doesn't work", will get you ignored. Posting a dozen lines of code, saying "after line 7 I was expecting to see &lt;x&gt;, but &lt;y&gt; occurred instead" is much more likely to get you a response. -->
당신이 만든 잘못된 코드에 대해서 도움을 요청할 때, 어떤 유형의 문제를 찾아봐야 하는지에 대한 아무런 힌트 없이 디버깅해달라고 하지 마세요. 몇백 줄짜리 코드만 적어놓고 "안 돼요"라고 하면 아무도 대답 하지 않을 겁니다. 열 몇 줄 정도 되는 코드를 올리며 "7번째 줄에서는 'x' 결과를 보는 걸 예상했는데 실제로는 'y'가 발생합니다" 같은 형식의 질문을 해야 답변받을 확률이 올라갑니다.

<!-- The most effective way to be precise about a code problem is to provide a minimal bug-demonstrating test case. What's a minimal test case? It's an illustration of the problem; just enough code to exhibit the undesirable behavior and no more. How do you make a minimal test case? If you know what line or section of code is producing the problematic behavior, make a copy of it and add just enough supporting code to produce a complete example (i.e. enough that the source is acceptable to the compiler/interpreter/whatever application processes it). If you can't narrow it down to a particular section, make a copy of the source and start removing chunks that don't affect the problematic behavior. The smaller your minimal test case is, the better (see [the section called “Volume is not precision”](#volume "Volume is not precision")). -->
코드 문제에 대해서 가장 정확하게 설명을 하는 방법은 해당 버그를 발생시키는 데 필요한 가장 간단한 테스트 케이스를 제공하는 겁니다. 가장 간단한 테스트 케이스가 뭘까요? 이는 책 안에 들어가는 삽화처럼 간단하게 문제를 묘사하는 것을 의미합니다. 원치 않는 행동을 하는 것을 보여줄 수 있는데 필요한 만큼만, 그 이상은 필요 없습니다. 어떻게 이런 간단한 테스트 케이스를 만들 수 있을까요? 특정 라인이나 섹션이 문제라는걸 알고 있다면, 그 부분을 복사해서 앞뒤로 최소한의 기능을 할 수 있도록 보강해서 하나의 완성된 예시로 만들면 됩니다. (다른 말로는, 컴파일러/인터프리터/기타 등등 에서 실행시킬 수 있는 코드를 의미합니다.) 문제가 되는 부분을 특정할 수 없다면, 코드를 통째로 복사를 한 다음에 문제가 되는 행동과 관련이 없는 부분들을 하나씩 지워 나가면서 범위를 좁혀나가면 됩니다. 문제를 나타내기 위한 최소한의 예시는 간단할수록 좋습니다. (["양보다는 질" 파트를 참조하세요.](#volume))

<!-- Generating a really small minimal test case will not always be possible, but trying to is good discipline. It may help you learn what you need to solve the problem on your own — and even when it doesn't, hackers like to see that you have tried. It will make them more cooperative. -->
아주 작은 테스트 케이스를 항상 만들 수 있는 것은 아니지만, 만들려고 시도 하는 것은 좋은 습관입니다. 스스로 문제를 해결하기 위해서 필요한 내용들을 배우는 데 도움이 되며, 결과적으로 스스로 문제를 해결하지 못하더라도 해커들은 당신이 시도했다는 것을 보고 싶어 합니다. 당신이 노력했다는 게 보이면 그들은 매우 협조적인 반응을 보일 겁니다.

<!-- If you simply want a code review, say as much up front, and be sure to mention what areas you think might particularly need review and why. -->
그냥 코드 리뷰를 받고 싶은 경우라면, 맨 처음에 코드 리뷰를 원한다고 써주세요. 어느 부분에서 집중적으로 리뷰를 받고 싶은지 적는 것도 까먹지 마세요.

<div id='homework'/>

<!-- ### Don't post homework questions -->
### 과제 물어보지 마세요

<!-- Hackers are good at spotting homework questions; most of us have done them ourselves. Those questions are for _you_ to work out, so that you will learn from the experience. It is OK to ask for hints, but not for entire solutions. -->
해커들은 과제로 나온 문제들을 집어내는데 일가견이 있습니다. 우리 중 대부분은 그런 과제들을 혼자서 해냈기 때문이죠. 해당 과제는 *당신이* 해결해야 하는 문제이며, 과제를 해결하는 과정을 통해 얻은 경험을 통해서 배우는 데 의미가 있는 겁니다. 우리에게 힌트를 요청하는 건 가능하지만, 전체 해답은 안 됩니다.

<!-- If you suspect you have been passed a homework question, but can't solve it anyway, try asking in a user group forum or (as a last resort) in a “user” list/forum of a project. While the hackers _will_ spot it, some of the advanced users may at least give you a hint. -->
정 못하겠다면 해커 포럼이 아닌 '사용자' 리스트/포럼에 물어보세요. 해커들은 *반드시* 눈치를 채겠지만, 실력 있는 사용자 중 몇 명은 힌트를 주려고 할 것입니다.

<div id='prune'/>

<!-- ### Prune pointless queries -->
### 거두절미

<!-- Resist the temptation to close your request for help with semantically-null questions like “Can anyone help me?” or “Is there an answer?” First: if you've written your problem description halfway competently, such tacked-on questions are at best superfluous. Second: because they are superfluous, hackers find them annoying — and are likely to return logically impeccable but dismissive answers like “Yes, you can be helped” and “No, there is no help for you.” -->
실질적인 의미를 가지지 않는, "도와주실 분 계시는가요?" 또는 "해결책이 있나요?" 같은 형식적인 질문으로 요청을 마무리하려는 마음은 접으셔야 합니다. 첫 번째 이유는, 당신이 어느 정도 문제를 잘 설명했다면 사족을 붙일 필요가 없습니다. 두 번째 이유는, 해당 문구는 사족이기에 해커들이 보면 짜증이 납니다. 따라서 논리적으로는 아무 문제가 없지만 당신을 철저히 무시하는 답변을 달 가능성이 높습니다. "도와주실 분 계시는가요?"에 "네" 또는 "아니요 없는데요" 같은 형식으로 말이죠.

<!-- In general, asking yes-or-no questions is a good thing to avoid unless you want a [yes-or-no answer](http://homepage.ntlworld.com./jonathan.deboynepollard/FGA/questions-with-yes-or-no-answers.html). -->
일반적으로, 반드시 예/아니오로 답변받으려는 경우가 아니라면 예/아니오 형태의 질문을 [지양하는 게 좋습니다.](<http://homepage.ntlworld.com./jonathan.deboynepollard/FGA/questions-with-yes-or-no-answers.html>).

<div id='urgent'/>

<!-- ### Don't flag your question as “Urgent”, even if it is for you -->
### 당신이 급하다고 "긴급" 말머리를 달지 마세요

<!-- That's your problem, not ours. Claiming urgency is very likely to be counter-productive: most hackers will simply delete such messages as rude and selfish attempts to elicit immediate and special attention. Furthermore, the word 'Urgent' (and other similar attempts to grab attention in the subject line) often triggers spam filters - your intended recipients might never see it at all! -->
당신 문제지 우리 알 바가 아닙니다. 긴급 상황이라고 주장하는 건 매우 비생산적인 행동일 가능성이 높습니다. 해커 대부분은 싸가지 없거나 이기적이며, 관심받으려고 하는 시도로 해석하여 즉시 메시지를 삭제할 겁니다. 더 나아가서, "긴급"이라는 단어 (또는 제목으로 관심을 끄는데 좋은 비슷한 단어들) 는 스팸 필터에 걸리는 경우가 다반사입니다. 당신이 의도한 수신 대상자들이 영영 보지 못할 수 있습니다!

<!-- There is one semi-exception. It can be worth mentioning if you're using the program in some high-profile place, one that the hackers will get excited about; in such a case, if you're under time pressure, and you say so politely, people may get interested enough to answer faster. -->
예외에 가까운 단 하나의 사례가 있다면, 당신이 해당 프로그램을 프로그램 제작자들이 듣기만 해도 재미를 느낄만한 굉장히 유명한 곳에서 사용하고 있다는 것을 밝히는 경우입니다. 이런 경우 시간의 압박에 쫓기고 있고, 예의 바르게 부탁한다면, 사람들의 이목이 쏠리고 답변을 빠르게 주려고 마음을 먹을 수 있습니다.

<!-- This is a very risky thing to do, however, because the hackers' metric for what is exciting probably differs from yours. Posting from the International Space Station would qualify, for example, but posting on behalf of a feel-good charitable or political cause would almost certainly not. In fact, posting “Urgent: Help me save the fuzzy baby seals!” will reliably get you shunned or flamed even by hackers who think fuzzy baby seals are important. -->
하지만, 이는 상당히 리스크가 큰 방법입니다. 해커들이 느끼는 재미의 척도는 보통 사람들과 다를 수 있기 때문입니다. 예를 들어 국제 우주 정거장에서 질문을 올리는 건 합격이지만, 자선단체나 정치적인 동기를 가진 단체를 언급한다면 확실히 불합격이라고 할 수 있습니다. 사실, "긴급: 귀여운 아기 물범들을 살리는 걸 도와주세요!" 같은 글을 올린다면 귀여운 아기 물범들이 중요하다고 생각하는 해커들한테서도 쌍욕을 먹을 겁니다.

<!-- If you find this mysterious, re-read the rest of this how-to repeatedly until you understand it before posting anything at all. -->
이게 잘 이해가 안 된다면, 절대 질문 글을 쓰면 안 됩니다. 앞의 내용을 포함한 나머지 내용들이 이해될 때까지 읽으세요.

<div id='courtesy'/>

<!-- ### Courtesy never hurts, and sometimes helps -->
### 정중해서 나쁠건 없습니다

<!-- Be courteous. Use “Please” and “Thanks for your attention” or “Thanks for your consideration”. Make it clear you appreciate the time people spend helping you for free. -->
정중하게 글을 작성하세요. "부탁드립니다", "관심을 가져주셔서 감사합니다", "생각 해주셔서 감사합니다" 등의 표현을 쓰세요. 당신을 무료로 도와주는 사람들이 당신을 도와주기 위해 시간을 내주는데 감사하다는 것을 확실하게 표현하세요.

<!-- To be honest, this isn't as important as (and cannot substitute for) being grammatical, clear, precise and descriptive, avoiding proprietary formats etc.; hackers in general would rather get somewhat brusque but technically sharp bug reports than polite vagueness. (If this puzzles you, remember that we value a question by what it teaches us.) -->
솔직히 말하자면 이것은 올바른 문법으로 명료하고 정확하게 묘사하며 올바른 첨부파일 형식을 갖추는 등의 행동보다 더 중요하지 않으며, 앞의 내용들을 대체할 수도 없습니다. 일반적으로 해커들은 무뚝뚝하지만, 기술적으로 날카로운 지적을 하는 버그 리포트를 예의 바르고 두루뭉술한 것보다 좋아합니다. (이게 잘 이해가 안 된다면, 우리는 그 질문을 통해서 우리가 배울 수 있는 것을 중요하게 여긴다는 걸 명심하세요.)

<!-- However, if you've got your technical ducks in a row, politeness does increase your chances of getting a useful answer. -->
하지만 당신이 앞서 말한 질문의 요소들을 다 갖추었다면, 정중하게 요청하는 건 유용한 답을 얻을 확률을 높여줍니다.

<!-- (We must note that the only serious objection we've received from veteran hackers to this HOWTO is with respect to our previous recommendation to use “Thanks in advance”. Some hackers feel this connotes an intention not to thank anybody afterwards. Our recommendation is to either say “Thanks in advance” first _and_ thank respondents afterwards, or express courtesy in a different way, such as by saying “Thanks for your attention” or “Thanks for your consideration”.) -->
(한 가지 공지를 해야 하는 것은, 해당 HOWTO 문서에서 베테랑 해커들에게서 유일하게 반대 의견을 받았던 부분은 이전 버전에서 추천했던 "Thanks in advance" 표현 관련 부분입니다. 일부 해커들은 해당 표현이 아무에게도 감사를 표하지 않는다는 뜻을 내포한다고 느끼기 때문입니다. 따라서 우리의 추천 방식은 "Thanks in advance"를 맨 처음에 쓰고 *반드시* 뒷부분에 다시 감사를 표하거나, 아니면 애초부터 다른 표현을 쓰는 것을 권장합니다. 예를 들어 "관심을 가져주셔서 감사합니다" 또는 "생각 해주셔서 감사합니다" 같은 표현들입니다.) (*역주: "Thank you in advance"는 사실상 실례가 되는 내용을 통보하고 양해를 구하는 식으로 많이 사용되는 표현입니다. 우리말로는 실례가 되는 내용을 통보할 때 맨 마지막에 "양해 해주셔서 감사합니다" 같은 식으로 사용되는 표현입니다.*)

<div id='followup'>

<!-- ### Follow up with a brief note on the solution -->
### 답변을 받고 나서 어떻게 됐는지 후속 상황을 알려주세요

<!-- Send a note after the problem has been solved to all who helped you; let them know how it came out and thank them again for their help. If the problem attracted general interest in a mailing list or newsgroup, it's appropriate to post the followup there. -->
질문글에 도움을 준 사람들에게 감사하다는 말을 남기세요. 어떻게 해결 되었는지를 말하고, 도움을 받아서 고맙다는걸 알리세요. 만약 메일링 리스트나 뉴스그룹 안에서 꽤 많은 사람들의 관심을 받았다면, 그곳에 후속 상황을 남기는게 좋습니다.

<!-- Optimally, the reply should be to the thread started by the original question posting, and should have ‘FIXED’, ‘RESOLVED’ or an equally obvious tag in the subject line. On mailing lists with fast turnaround, a potential respondent who sees a thread about “Problem X” ending with “Problem X - FIXED” knows not to waste his/her time even reading the thread (unless (s)he personally finds Problem X interesting) and can therefore use that time solving a different problem. -->
제일 좋은 상황은, 원래 질문글 스레드에 'FIXED', 'RESOLVED'와 같은 명확한 태그와 함께 답글을 남기는 것 입니다. 회전율이 높은 메일링 리스트의 경우, 답변을 달려고 하는 사람이 해당 스레드가 "문제 X" 로 시작해서 "문제 X - FIXED" 같은 형태로 끝나는 것을 파악한다면, 이미 해결이 끝난 문제임을 파악하여 스레드를 읽느라 시간을 낭비하지 않으며 (개인적으로 해당 문제 X에 대해서 흥미를 느끼지 않는 경우) 다른 문제를 해결하는데 시간을 할애할 수 있습니다.

<!-- Your followup doesn't have to be long and involved; a simple “Howdy — it was a failed network cable! Thanks, everyone. - Bill” would be better than nothing. In fact, a short and sweet summary is better than a long dissertation unless the solution has real technical depth. Say what action solved the problem, but you need not replay the whole troubleshooting sequence. -->
팔로우업을 길게 공들여서 쓸 필요는 없습니다. 간단하게 "안녕하세요 - 네트워크 케이블이 망가져서 생긴 문제였습니다! 도와주신 분들 감사합니다. - 홍길동" 는 충분히 아무 말이 없는 것 보다는 낫습니다. 사실 해결 방법이 엄청나게 기술적으로 심도있는 내용이 아니라면 짧게 잘 요약된 글이 논문처럼 긴 글보다 낫습니다. 어떤 행동이 문제 해결로 이어지는지 적되, 전체 해결 방법을 전부 다 설명 할 필요는 없습니다.

<!-- TODO: 여기서부터 -->
<!-- For problems with some depth, it is appropriate to post a summary of the troubleshooting history. Describe your final problem statement. Describe what worked as a solution, and indicate avoidable blind alleys _after that_. The blind alleys should come after the correct solution and other summary material, rather than turning the follow-up into a detective story. Name the names of people who helped you; you'll make friends that way. -->
심도있는 문제에 대해서는 문제 해결을 하는 과정 전체를 요약한 글을 올리는게 좋습니다. 결국 무엇이 문제였는지 적어주세요. 어떤 방법이 해결책으로 작용했고, *해결책을 적은 후에* 해결책을 찾으면서 잘못 들어섰던 막다른 길들을 미리 알고 피해갈 수 있도록 소개해야 합니다. 이런 막다른 길들은 올바른 해결책과 기타 요점들 이후에 제시 되어야지, 그렇지 않으면 글이 탐정 추리물이 되어버립니다. 도와준 사람들의 이름을 언급하세요. 그러면서 친구들을 만들 수 있을겁니다.

<!-- Besides being courteous and informative, this sort of followup will help others searching the archive of the mailing-list/newsgroup/forum to know exactly which solution helped you and thus may also help them. -->
정중한 태도와 알찬 내용을 떠나서, 이런 형태로 팔로우업을 쓰게 되면 다른 사람들이 메일링 리스트/뉴스그룹/포럼 의 과거 기록을 검색할 때 정확히 어떤 해결책이 당신에게 도움이 되었는지 쉽게 알 수 있도록 도움이 되고, 그 사람들에게 도움이 될겁니다.

<!-- Last, and not least, this sort of followup helps everybody who assisted feel a satisfying sense of closure about the problem. If you are not a techie or hacker yourself, trust us that this feeling is very important to the gurus and experts you tapped for help. Problem narratives that trail off into unresolved nothingness are frustrating things; hackers itch to see them resolved. The goodwill that scratching that itch earns you will be very, very helpful to you next time you need to pose a question. -->
마지막으로 중요한 이유 하나를 얘기하자면, 이런 식으로 후기를 작성하게 되면 도움을 준 사람들이 문제가 해결 되었다는 것을 알게 되어서 후련함을 느낍니다. 당신이 techie나 해커가 아니라서 이게 그렇게 중요한지 잘 모르겠다면, 우리를 믿어야 합니다. 당신들이 도움을 달라고 했던 현자(guru)들이나 전문가들 에게는 매우 중요합니다. 문제 상황이 계속 되어서 

Consider how you might be able to prevent others from having the same problem in the future. Ask yourself if a documentation or FAQ patch would help, and if the answer is yes send that patch to the maintainer.

Among hackers, this sort of good followup behavior is actually more important than conventional politeness. It's how you get a reputation for playing well with others, which can be a very valuable asset.

How To Interpret Answers
------------------------

### RTFM and STFW: How To Tell You've Seriously Screwed Up

There is an ancient and hallowed tradition: if you get a reply that reads “RTFM”, the person who sent it thinks you should have Read The Fucking Manual. He or she is almost certainly right. Go read it.

RTFM has a younger relative. If you get a reply that reads “STFW”, the person who sent it thinks you should have Searched The Fucking Web. He or she is almost certainly right. Go search it. (The milder version of this is when you are told “Google is your friend!”)

In Web forums, you may also be told to search the forum archives. In fact, someone may even be so kind as to provide a pointer to the previous thread where this problem was solved. But do not rely on this consideration; do your archive-searching before asking.

Often, the person telling you to do a search has the manual or the web page with the information you need open, and is looking at it as he or she types. These replies mean that the responder thinks (a) the information you need is easy to find, and (b) you will learn more if you seek out the information than if you have it spoon-fed to you.

You shouldn't be offended by this; by hacker standards, your respondent is showing you a rough kind of respect simply by not ignoring you. You should instead be thankful for this grandmotherly kindness.

### If you don't understand

If you don't understand the answer, do not immediately bounce back a demand for clarification. Use the same tools that you used to try and answer your original question (manuals, FAQs, the Web, skilled friends) to understand the answer. Then, if you still need to ask for clarification, exhibit what you have learned.

For example, suppose I tell you: “It sounds like you've got a stuck zentry; you'll need to clear it.” Then: here's a _bad_ followup question: “What's a zentry?” Here's a _good_ followup question: “OK, I read the man page and zentries are only mentioned under the -z and -p switches. Neither of them says anything about clearing zentries. Is it one of these or am I missing something here?”

### Dealing with rudeness

Much of what looks like rudeness in hacker circles is not intended to give offense. Rather, it's the product of the direct, cut-through-the-bullshit communications style that is natural to people who are more concerned about solving problems than making others feel warm and fuzzy.

When you perceive rudeness, try to react calmly. If someone is really acting out, it is very likely a senior person on the list or newsgroup or forum will call him or her on it. If that _doesn't_ happen and you lose your temper, it is likely that the person you lose it at was behaving within the hacker community's norms and _you_ will be considered at fault. This will hurt your chances of getting the information or help you want.

On the other hand, you will occasionally run across rudeness and posturing that is quite gratuitous. The flip-side of the above is that it is acceptable form to slam real offenders quite hard, dissecting their misbehavior with a sharp verbal scalpel. Be very, very sure of your ground before you try this, however. The line between correcting an incivility and starting a pointless flamewar is thin enough that hackers themselves not infrequently blunder across it; if you are a newbie or an outsider, your chances of avoiding such a blunder are low. If you're after information rather than entertainment, it's better to keep your fingers off the keyboard than to risk this.

(Some people assert that many hackers have a mild form of autism or Asperger's Syndrome, and are actually missing some of the brain circuitry that lubricates “normal” human social interaction. This may or may not be true. If you are not a hacker yourself, it may help you cope with our eccentricities if you think of us as being brain-damaged. Go right ahead. We won't care; we _like_ being whatever it is we are, and generally have a healthy skepticism about clinical labels.)

Jeff Bigler's observations about [tact filters](http://www.mit.edu/~jcb/tact.html) are also relevant and worth reading.

In the next section, we'll talk about a different issue; the kind of “rudeness” you'll see when _you_ misbehave.

On Not Reacting Like A Loser
----------------------------

Odds are you'll screw up a few times on hacker community forums — in ways detailed in this article, or similar. And you'll be told exactly how you screwed up, possibly with colourful asides. In public.

When this happens, the worst thing you can do is whine about the experience, claim to have been verbally assaulted, demand apologies, scream, hold your breath, threaten lawsuits, complain to people's employers, leave the toilet seat up, etc. Instead, here's what you do:

Get over it. It's normal. In fact, it's healthy and appropriate.

Community standards do not maintain themselves: They're maintained by people actively applying them, visibly, _in public_. Don't whine that all criticism should have been conveyed via private e-mail: That's not how it works. Nor is it useful to insist you've been personally insulted when someone comments that one of your claims was wrong, or that his views differ. Those are loser attitudes.

There have been hacker forums where, out of some misguided sense of hyper-courtesy, participants are banned from posting any fault-finding with another's posts, and told “Don't say anything if you're unwilling to help the user.” The resulting departure of clueful participants to elsewhere causes them to descend into meaningless babble and become useless as technical forums.

Exaggeratedly “friendly” (in that fashion) or useful: Pick one.

Remember: When that hacker tells you that you've screwed up, and (no matter how gruffly) tells you not to do it again, he's acting out of concern for (1) you and (2) his community. It would be much easier for him to ignore you and filter you out of his life. If you can't manage to be grateful, at least have a little dignity, don't whine, and don't expect to be treated like a fragile doll just because you're a newcomer with a theatrically hypersensitive soul and delusions of entitlement.

Sometimes people will attack you personally, flame without an apparent reason, etc., even if you don't screw up (or have only screwed up in their imagination). In this case, complaining is the way to _really_ screw up.

These flamers are either lamers who don't have a clue but believe themselves to be experts, or would-be psychologists testing whether you'll screw up. The other readers either ignore them, or find ways to deal with them on their own. The flamers' behavior creates problems for themselves, which don't have to concern you.

Don't let yourself be drawn into a flamewar, either. Most flames are best ignored — after you've checked whether they are really flames, not pointers to the ways in which you have screwed up, and not cleverly ciphered answers to your real question (this happens as well).

Questions Not To Ask
--------------------

Here are some classic stupid questions, and what hackers are thinking when they don't answer them.

Q: [Where can I find program or resource X?](#idm551)

Q: [How can I use X to do Y?](#idm557)

Q: [How can I configure my shell prompt?](#idm562)

Q: [Can I convert an AcmeCorp document into a TeX file using the Bass-o-matic file converter?](#idm568)

Q: [My {program, configuration, SQL statement} doesn't work](#idm573)

Q: [I'm having problems with my Windows machine. Can you help?](#idm585)

Q: [My program doesn't work. I think system facility X is broken.](#idm592)

Q: [I'm having problems installing Linux or X. Can you help?](#idm597)

Q: [How can I crack root/steal channel-ops privileges/read someone's e-mail?](#idm606)

|     |     |
| --- | --- |
| **Q:** | Where can I find program or resource X? |
| **A:** | The same place I'd find it, fool — at the other end of a web search. Ghod, doesn't everybody know how to use [Google](http://www.google.com/) yet? |
| **Q:** | How can I use X to do Y? |
| **A:** | If what you want is to do Y, you should ask that question without pre-supposing the use of a method that may not be appropriate. Questions of this form often indicate a person who is not merely ignorant about X, but confused about what problem Y they are solving and too fixated on the details of their particular situation. It is generally best to ignore such people until they define their problem better. |
| **Q:** | How can I configure my shell prompt? |
| **A:** | If you're smart enough to ask this question, you're smart enough to [RTFM](#rtfm "RTFM and STFW: How To Tell You've Seriously Screwed Up") and find out yourself. |
| **Q:** | Can I convert an AcmeCorp document into a TeX file using the Bass-o-matic file converter? |
| **A:** | Try it and see. If you did that, you'd (a) learn the answer, and (b) stop wasting my time. |
| **Q:** | My {program, configuration, SQL statement} doesn't work |
| **A:** | This is not a question, and I'm not interested in playing Twenty Questions to pry your actual question out of you — I have better things to do. On seeing something like this, my reaction is normally of one of the following:<br><br>*do you have anything else to add to that?<br>    <br>* oh, that's too bad, I hope you get it fixed.<br>    <br>* and this has exactly what to do with me? |
| **Q:** | I'm having problems with my Windows machine. Can you help? |
| **A:** | Yes. Throw out that Microsoft trash and install an open-source operating system like Linux or BSD.<br><br>Note: you _can_ ask questions related to Windows machines if they are about a program that does have an official Windows build, or interacts with Windows machines (i.e., Samba). Just don't be surprised by the reply that the problem is with Windows and not the program, because Windows is so broken in general that this is very often the case. |
| **Q:** | My program doesn't work. I think system facility X is broken. |
| **A:** | While it is possible that you are the first person to notice an obvious deficiency in system calls and libraries heavily used by hundreds or thousands of people, it is rather more likely that you are utterly clueless. Extraordinary claims require extraordinary evidence; when you make a claim like this one, you must back it up with clear and exhaustive documentation of the failure case. |
| **Q:** | I'm having problems installing Linux or X. Can you help? |
| **A:** | No. I'd need hands-on access to your machine to troubleshoot this. Go ask your local Linux user group for hands-on help. (You can find a list of user groups [here](http://www.linux.org/groups/index.html).)<br><br>Note: questions about installing Linux may be appropriate if you're on a forum or mailing list about a particular distribution, and the problem is with _that_ distro; or on local user groups forums. In this case, be sure to describe the exact details of the failure. But do careful searching first, with "linux" and _all_ suspicious pieces of hardware. |
| **Q:** | How can I crack root/steal channel-ops privileges/read someone's e-mail? |
| **A:** | You're a lowlife for wanting to do such things and a moron for asking a hacker to help you. |

Good and Bad Questions
----------------------

Finally, I'm going to illustrate how to ask questions in a smart way by example; pairs of questions about the same problem, one asked in a stupid way and one in a smart way.

**Stupid:** Where can I find out stuff about the Foonly Flurbamatic?

This question just begs for ["STFW"](#rtfm "RTFM and STFW: How To Tell You've Seriously Screwed Up") as a reply.

**Smart:** I used Google to try to find “Foonly Flurbamatic 2600” on the Web, but I got no useful hits. Can I get a pointer to programming information on this device?

This one has already STFWed, and sounds like there might be a real problem.

**Stupid:** I can't get the code from project foo to compile. Why is it broken?

The querent assumes that somebody else screwed up. Arrogant git...

**Smart:** The code from project foo doesn't compile under Nulix version 6.2. I've read the FAQ, but it doesn't have anything in it about Nulix-related problems. Here's a transcript of my compilation attempt; is it something I did?

The querent has specified the environment, read the FAQ, is showing the error, and is not assuming his problems are someone else's fault. This one might be worth some attention.

**Stupid:** I'm having problems with my motherboard. Can anybody help?

J. Random Hacker's response to this is likely to be “Right. Do you need burping and diapering, too?” followed by a punch of the delete key.

**Smart:** I tried X, Y, and Z on the S2464 motherboard. When that didn't work, I tried A, B, and C. Note the curious symptom when I tried C. Obviously the florbish is grommicking, but the results aren't what one might expect. What are the usual causes of grommicking on Athlon MP motherboards? Anybody got ideas for more tests I can run to pin down the problem?

This person, on the other hand, seems worthy of an answer. He/she has exhibited problem-solving intelligence rather than passively waiting for an answer to drop from on high.

In the last question, notice the subtle but important difference between demanding “Give me an answer” and “Please help me figure out what additional diagnostics I can run to achieve enlightenment.”

In fact, the form of that last question is closely based on a real incident that happened in August 2001 on the linux-kernel mailing list (lkml). I (Eric) was the one asking the question that time. I was seeing mysterious lockups on a Tyan S2462 motherboard. The list members supplied the critical information I needed to solve them.

By asking the question in the way I did, I gave people something to chew on; I made it easy and attractive for them to get involved. I demonstrated respect for my peers' ability and invited them to consult with me as a peer. I also demonstrated respect for the value of their time by telling them the blind alleys I had already run down.

Afterwards, when I thanked everyone and remarked how well the process had worked, an lkml member observed that he thought it had worked not because I'm a “name” on that list, but because I asked the question in the proper form.

Hackers are in some ways a very ruthless meritocracy; I'm certain he was right, and that if I _had_ behaved like a sponge I would have been flamed or ignored no matter who I was. His suggestion that I write up the whole incident as instruction to others led directly to the composition of this guide.

If You Can't Get An Answer
--------------------------

If you can't get an answer, please don't take it personally that we don't feel we can help you. Sometimes the members of the asked group may simply not know the answer. No response is not the same as being ignored, though admittedly it's hard to spot the difference from outside.

In general, simply re-posting your question is a bad idea. This will be seen as pointlessly annoying. Have patience: the person with your answer may be in a different time-zone and asleep. Or it may be that your question wasn't well-formed to begin with.

There are other sources of help you can go to, often sources better adapted to a novice's needs.

There are many online and local user groups who are enthusiasts about the software, even though they may never have written any software themselves. These groups often form so that people can help each other and help new users.

There are also plenty of commercial companies you can contract with for help, both large and small. Don't be dismayed at the idea of having to pay for a bit of help! After all, if your car engine blows a head gasket, chances are you would take it to a repair shop and pay to get it fixed. Even if the software didn't cost you anything, you can't expect that support to always come for free.

For popular software like Linux, there are at least 10,000 users per developer. It's just not possible for one person to handle the support calls from over 10,000 users. Remember that even if you have to pay for support, you are still paying much less than if you had to buy the software as well (and support for closed-source software is usually more expensive and less competent than support for open-source software).

How To Answer Questions in a Helpful Way
----------------------------------------

_Be gentle._ Problem-related stress can make people seem rude or stupid even when they're not.

_Reply to a first offender off-line._ There is no need of public humiliation for someone who may have made an honest mistake. A real newbie may not know how to search archives or where the FAQ is stored or posted.

_If you don't know for sure, say so!_ A wrong but authoritative-sounding answer is worse than none at all. Don't point anyone down a wrong path simply because it's fun to sound like an expert. Be humble and honest; set a good example for both the querent and your peers.

_If you can't help, don't hinder._ Don't make jokes about procedures that could trash the user's setup — the poor sap might interpret these as instructions.

_Ask probing questions to elicit more details._ If you're good at this, the querent will learn something — and so might you. Try to turn the bad question into a good one; remember we were all newbies once.

While muttering RTFM is sometimes justified when replying to someone who is just a lazy slob, a pointer to documentation (even if it's just a suggestion to google for a key phrase) is better.

_If you're going to answer the question at all, give good value._ Don't suggest kludgy workarounds when somebody is using the wrong tool or approach. Suggest good tools. Reframe the question.

Answer the actual question! If the querent has been so thorough as to do his or her research and has included in the query that X, Y, Z, A, B, and C have already been tried without good result, it is supremely unhelpful to respond with “Try A or B,” or with a link to something that only says, “Try X, Y, Z, A, B, or C.”.

_Help your community learn from the question._ When you field a good question, ask yourself “How would the relevant documentation or FAQ have to change so that nobody has to answer this again?” Then send a patch to the document maintainer.

If you did research to answer the question, _demonstrate your skills rather than writing as though you pulled the answer out of your butt._ Answering one good question is like feeding a hungry person one meal, but teaching them research skills by example is showing them how to grow food for a lifetime.

Related Resources
-----------------

If you need instruction in the basics of how personal computers, Unix, and the Internet work, see [The Unix and Internet Fundamentals HOWTO](http://en.tldp.org/HOWTO/Unix-and-Internet-Fundamentals-HOWTO/).

When you release software or write patches for software, try to follow the guidelines in the [Software Release Practice HOWTO](http://en.tldp.org/HOWTO/Software-Release-Practice-HOWTO/index.html).

Acknowledgements
----------------

Evelyn Mitchell contributed some example stupid questions and inspired the “How To Give A Good Answer” section. Mikhail Ramendik contributed some particularly valuable suggestions for improvements.


Revision History
------------------
|     |     |     |
| --- | --- | --- |
| Revision 3.10 | 21 May 2014 | esr |
| New section on Stack Overflow. |     |     |
| Revision 3.9 | 23 Apr 2013 | esr |
| URL fixes. |     |     |
| Revision 3.8 | 19 Jun 2012 | esr |
| URL fix. |     |     |
| Revision 3.7 | 06 Dec 2010 | esr |
| Helpful hints for ESL speakers. |     |     |
| Revision 3.7 | 02 Nov 2010 | esr |
| Several translations have disappeared. |     |     |
| Revision 3.6 | 19 Mar 2008 | esr |
| Minor update and new links. |     |     |
| Revision 3.5 | 2 Jan 2008 | esr |
| Typo fix and some translation links. |     |     |
| Revision 3.4 | 24 Mar 2007 | esr |
| New section, "When asking about code". |     |     |
| Revision 3.3 | 29 Sep 2006 | esr |
| Folded in a good suggestion from Kai Niggemann. |     |     |
| Revision 3.2 | 10 Jan 2006 | esr |
| Folded in edits from Rick Moen. |     |     |
| Revision 3.1 | 28 Oct 2004 | esr |
| Document 'Google is your friend!' |     |     |
| Revision 3.0 | 2 Feb 2004 | esr |
| Major addition of stuff about proper etiquette on Web forums. |     |     |

* * *
