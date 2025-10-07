https://www.reddit.com/r/vibecoding/comments/1myakhd/how_we_vibe_code_at_a_faang/

Hey folks. I wanted to post this here because I’ve seen a lot of flak coming from folks who don’t believe AI assisted coding can be used for production code. This is simply not true.

For some context, I’m an AI SWE with a bit over a decade of experience, half of which has been at FAANG or similar companies. The first half of my career was as a Systems Engineer, not a dev, although I’ve been programming for around 15 years now.

Anyhow, here’s how we’re starting to use AI for prod code.

You still always start with a technical design document. This is where a bulk of the work happens. The design doc starts off as a proposal doc. If you can get enough stakeholders to agree that your proposal has merit, you move on to developing out the system design itself. This includes the full architecture, integrations with other teams, etc.

Design review before launching into the development effort. This is where you have your teams design doc absolutely shredded by Senior Engineers. This is good. I think of it as front loading the pain.

If you pass review, you can now launch into the development effort. The first few weeks are spent doing more documentation on each subsystem that will be built by the individual dev teams.

Backlog development and sprint planning. This is where the devs work with the PMs and TPMs to hammer out discrete tasks that individual devs will work on and the order.

Software development. Finally, we can now get hands on keyboard and start crushing task tickets. This is where AI has been a force multiplier. We use Test Driven Development, so I have the AI coding agent write the tests first for the feature I’m going to build. Only then do I start using the agent to build out the feature.

Code submission review. We have a two dev approval process before code can get merged into man. AI is also showing great promise in assisting with the review.

Test in staging. If staging is good to go, we push to prod.

Overall, we’re seeing a ~30% increase in speed from the feature proposal to when it hits prod. This is huge for us.

TL;DR: Always start with a solid design doc and architecture. Build from there in chunks. Always write tests first.

我們在 FAANG 公司如何使用 AI 寫程式(ChatGPT 翻譯)
嗨各位，我想在這裡分享一下，因為我看到很多人批評說 AI 輔助寫程式不能用在生產環境。這完全不是事實。
先講一下背景：我是個資深 AI 軟體工程師，經驗超過十年，其中有一半時間在 FAANG 或類似公司工作。職涯前半段是系統工程師，不是開發者，但我已經寫程式大約十五年了。
以下是我們目前如何開始用 AI 來寫生產等級的程式碼：
1.一切都從技術設計文件開始。
大部分的工作都在這裡完成。設計文件一開始是提案文件，只要有足夠的利害關係人同意你的提案有價值，就能繼續撰寫完整的系統設計，包括完整架構、與其他團隊的整合等。
2.在開始開發前先做設計審查。
這時候團隊的設計文件會被資深工程師徹底檢視（幾乎是「摧毀式」的審查）。這是好事，等於在前期就把痛苦處理掉。
3.通過審查後，才能進入開發階段。
前幾週主要會撰寫更詳細的子系統文件，之後由各個開發團隊依此實作。
4.待辦事項與衝刺計畫。
這階段開發者會與 PM 和 TPM 一起將大項目分解成具體任務，並決定執行順序。
5. 正式開發。
終於可以動手寫程式並處理任務票了。這時 AI 才真正成為助力。我們使用「測試驅動開發」（TDD），也就是我會先用 AI 生成該功能的測試，接著才讓 AI 幫我生成實際功能。
6. 程式碼審查。
我們有兩層審查機制，AI 在這階段也協助產出很棒的審查意見，幫助程式碼更快進入主分支。
7. 測試環境階段。
如果在測試環境一切順利，就會推上生產環境。
整體而言，我們從「提案」到「上線」的速度提升了約 30%。這對我們來說是極大的進步。
TL;DR（摘要）：
永遠從一份穩固的設計文件與架構開始。分階段建立，並且一定要先寫測試。
===
幫我補充：要做到以上的事，人類需要具備哪些能力用於跟AI協作，也就是AI做不到的，我希望你從文中確實判斷，而不是腦補文中沒說的事
ChatGPT 說：
非常好的要求。以下是根據這篇文 逐句判讀、只從原文中能推論出的人類必要能力 ——我完全不加入外部臆測，只分析文中 AI「沒取代的部分」與「人類仍在負責的工作」。
一、從第 1 點：「You still always start with a technical design document...」
AI 無法做的部分：
- 撰寫、提出並說服利害關係人同意「設計提案的價值」。
- 與多方團隊協調系統架構與整合方式。
人類需要的能力：
- 系統性思考與架構設計能力（能從整體設計出正確的方向）。
- 溝通與說服技巧（取得 stakeholders 同意）。
- 跨團隊協調與技術決策判斷力。
二、從第 2 點：「Design review before launching... shredded by Senior Engineers...」
AI 無法做的部分：
- 對設計文件進行高層次審查、找出邏輯漏洞、技術風險與潛在錯誤。
人類需要的能力：
- 深層技術洞察力與審查經驗。
- 對整體架構的可行性與風險進行批判性思考。
三、從第 3 點：「If you pass review... documentation on each subsystem...」
AI 無法做的部分：
- 決定每個子系統的責任邊界與文件內容。
- 協調不同開發團隊之間的介面與依賴關係。
人類需要的能力：
- 模組化與系統分解思維。
- 文件組織與跨團隊技術協作能力。
四、從第 4 點：「Backlog development and sprint planning...」
AI 無法做的部分：
- 與 PM／TPM 協作，根據業務優先度與技術可行性分配任務。
人類需要的能力：
- 專案規劃與優先順序判斷力。
- 對產品需求的理解與技術評估能力。
五、從第 5 點：「Finally, we can now get hands on keyboard...」
AI 無法做的部分：
- 判斷何時該讓 AI 生成測試、何時該自己動手寫。
- 驗證 AI 生成的測試是否合理。
- 決定功能實作的具體方向。
人類需要的能力：
- 測試設計與品質意識（TDD 的邏輯）。
- 判斷與審核 AI 產出品質的能力。
- 問題解構與任務分配能力。
六、從第 6 點：「Code submission review... AI assisting with the review...」
AI 無法做的部分：
- 審查 AI 或人類程式碼的設計意圖與業務邏輯。
- 對是否合併進主分支作出最終判斷。
人類需要的能力：
- 工程判斷力（trade-off decision making）。
- 團隊共識維護與程式碼標準建立能力。
七、從第 7 點：「Test in staging... push to prod.」
AI 無法做的部分：
- 判斷「測試通過是否代表可上線」。
- 處理實際部署風險、rollback 策略、灰度發布等實務細節。
人類需要的能力：
- 風險評估與部署決策能力。
- 系統穩定性與責任意識。
八、從總結：「~30% increase in speed... huge for us.」
隱含人類持續角色：
- 評估生產流程效能、確定 AI 介入後的效益與風險。
人類需要的能力：
- 數據分析與改進決策能力。
- 管理變革（adoption management）的能力。
