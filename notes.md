26. 如果換成你現在腦中的「傷害帳本」
假設 agent 一直產生成果：
\[
a_1,a_2,a_3,\ldots
\]
每個 action 有 harm：
\[
h_1,h_2,h_3,\ldots
\]
Budgeted RL 最接近的是：
\[
G_h
=
\sum_t\gamma^th_t
\]
再限制：
\[
\mathbb E[G_h]\le\beta
\]
也就是：
整段行為的 expected 累積 harm 不能超過人類指定的 budget。

但如果你腦中的規則是：
「歷史已造成 harm = 7，總上限是 10，因此任何 future action 都絕對不能讓 realized cumulative harm > 10。」

那已經比這篇的基本 formulation 更強。
如果你想的是：
「任何單次 action harm 都不得 > 3。」

那又是另一種 constraint。
如果你想的是：
「一旦 irreversible harm 發生，就永遠算在帳上，而且不得被未來好事抵銷。」

那又多了一層結構。
這就是為什麼你下一篇 Irreversibility Budget 接得非常漂亮。