<div class="Box-sc-g0xbh4-0 QkQOb js-snippet-clipboard-copy-unpositioned" data-hpc="true"><article class="markdown-body entry-content container-lg" itemprop="text"><div class="markdown-heading" dir="auto"><h1 tabindex="-1" class="heading-element" dir="auto" _msttexthash="9751534" _msthash="279">呼叫中心 AI</h1><a id="user-content-call-center-ai" class="anchor" aria-label="永久链接：呼叫中心 AI" href="#call-center-ai" _mstaria-label="475969" _msthash="280"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto" _msttexthash="143856947" _msthash="281">使用 Azure 和 OpenAI GPT 的 AI 驱动的呼叫中心解决方案。</p>

<p dir="auto"><a href="https://github.com/clemlesne/call-center-ai/releases"><img src="https://camo.githubusercontent.com/517833d250f296937a629ba1110df1bd095ea31cfae4818c15b1b9c6687d6479/68747470733a2f2f696d672e736869656c64732e696f2f6769746875622f72656c656173652d646174652f636c656d6c65736e652f63616c6c2d63656e7465722d6169" alt="上次发布日期" data-canonical-src="https://img.shields.io/github/release-date/clemlesne/call-center-ai" style="max-width: 100%;" _mstalt="284479" _msthash="282"></a>
<a href="https://github.com/clemlesne/call-center-ai/blob/main/LICENSE"><img src="https://camo.githubusercontent.com/1e4a688d90f271a48495a29dd845cd895f54ead151490479fd51b0f26a5ff547/68747470733a2f2f696d672e736869656c64732e696f2f6769746875622f6c6963656e73652f636c656d6c65736e652f63616c6c2d63656e7465722d6169" alt="项目许可证" data-canonical-src="https://img.shields.io/github/license/clemlesne/call-center-ai" style="max-width: 100%;" _mstalt="258843" _msthash="283"></a></p>

<p dir="auto"><a href="https://codespaces.new/microsoft/call-center-ai?quickstart=1" rel="nofollow"><img src="https://github.com/codespaces/badge.svg" alt="在 GitHub Codespaces 中打开" style="max-width: 100%;" _mstalt="507845" _msthash="284"></a></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto" _msttexthash="6290102" _msthash="285">概述</h2><a id="user-content-overview" class="anchor" aria-label="永久链接： 概述" href="#overview" _mstaria-label="375934" _msthash="286"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto" _msttexthash="349860615" _msthash="287">在 API 调用中从 AI 代理发送电话呼叫。或者，直接从配置的电话号码呼叫机器人！</p>
<p dir="auto" _msttexthash="406046108" _msthash="288">保险、IT 支持、客户服务等。机器人可以在几秒钟内（真的）进行自定义以满足您的需求。</p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-c"><span class="pl-c">#</span> Ask the bot to call a phone number</span>
data=<span class="pl-s"><span class="pl-pds">'</span>{</span>
<span class="pl-s">  "bot_company": "Contoso",</span>
<span class="pl-s">  "bot_name": "Amélie",</span>
<span class="pl-s">  "phone_number": "+11234567890",</span>
<span class="pl-s">  "task": "Help the customer with their digital workplace. Assistant is working for the IT support department. The objective is to help the customer with their issue and gather information in the claim.",</span>
<span class="pl-s">  "agent_phone_number": "+33612345678",</span>
<span class="pl-s">  "claim": [</span>
<span class="pl-s">    {</span>
<span class="pl-s">      "name": "hardware_info",</span>
<span class="pl-s">      "type": "text"</span>
<span class="pl-s">    },</span>
<span class="pl-s">    {</span>
<span class="pl-s">      "name": "first_seen",</span>
<span class="pl-s">      "type": "datetime"</span>
<span class="pl-s">    },</span>
<span class="pl-s">    {</span>
<span class="pl-s">      "name": "building_location",</span>
<span class="pl-s">      "type": "text"</span>
<span class="pl-s">    }</span>
<span class="pl-s">  ]</span>
<span class="pl-s">}<span class="pl-pds">'</span></span>

curl \
  --header <span class="pl-s"><span class="pl-pds">'</span>Content-Type: application/json<span class="pl-pds">'</span></span> \
  --request POST \
  --url https://xxx/call \
  --data <span class="pl-smi">$data</span></pre><div class="zeroclipboard-container">
     
  </div></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto" _msttexthash="5209451" _msthash="289">特征</h3><a id="user-content-features" class="anchor" aria-label="永久链接：功能" href="#features" _mstaria-label="370552" _msthash="290"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="markdown-alert markdown-alert-note" dir="auto"><p class="markdown-alert-title" dir="auto"><svg class="octicon octicon-info mr-2" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="M0 8a8 8 0 1 1 16 0A8 8 0 0 1 0 8Zm8-6.5a6.5 6.5 0 1 0 0 13 6.5 6.5 0 0 0 0-13ZM6.5 7.75A.75.75 0 0 1 7.25 7h1a.75.75 0 0 1 .75.75v2.75h.25a.75.75 0 0 1 0 1.5h-2a.75.75 0 0 1 0-1.5h.25v-2h-.25a.75.75 0 0 1-.75-.75ZM8 6a1 1 0 1 1 0-2 1 1 0 0 1 0 2Z"></path></svg><font _mstmutation="1" _msttexthash="5121168" _msthash="291">注意</font></p><p dir="auto" _msttexthash="748761143" _msthash="292">这个项目是一个概念验证。它不打算用于生产。这演示了如何结合使用 Azure 通信服务、Azure 认知服务和 Azure OpenAI 来构建自动化呼叫中心解决方案。</p>
</div>
<ul class="contains-task-list">
<li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox" checked=""><font _mstmutation="1" _msttexthash="45291935" _msthash="293">在公共网站上访问索赔</font></li>
<li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox" checked=""><font _mstmutation="1" _msttexthash="41787122" _msthash="294">访问客户对话历史记录</font></li>
<li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox" checked=""><font _mstmutation="1" _msttexthash="51871924" _msthash="295">允许用户更改对话的语言</font></li>
<li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox" checked=""><font _mstmutation="1" _msttexthash="108346446" _msthash="296">Assistant 可以向用户发送 SMS 以获取更多信息</font></li>
<li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox" checked=""><font _mstmutation="1" _msttexthash="36419266" _msthash="297">可以从电话号码调用 Bot</font></li>
<li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox" checked=""><font _mstmutation="1" _msttexthash="270886330" _msthash="298">机器人使用多种语音音调（例如，happy、sad、neutral）来保持对话的吸引力</font></li>
<li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox" checked=""><font _mstmutation="1" _msttexthash="270638121" _msthash="299">机器人可以理解公司产品（= 词典）（例如，特定保险产品的名称）</font></li>
<li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox" checked=""><font _mstmutation="1" _msttexthash="107385395" _msthash="300">自行创建一个任务的待办事项列表以完成声明</font></li>
<li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox" checked=""><font _mstmutation="1" _msttexthash="24332607" _msthash="301">可自定义的提示</font></li>
<li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox" checked=""><font _mstmutation="1" _msttexthash="35661990" _msthash="302">需要时脱离人工代理</font></li>
<li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox" checked=""><font _mstmutation="1" _msttexthash="218248667" _msthash="303">从 LLM 中过滤掉不适当的内容，例如亵渎性语言或同意的公司名称</font></li>
<li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox" checked=""><font _mstmutation="1" _msttexthash="92761344" _msthash="304">使用 GPT-4o 和 GPT 4o-mini 深入了解客户要求</font></li>
<li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox" checked=""><font _mstmutation="1" _msttexthash="45914323" _msthash="305">遵循声明的特定数据架构</font></li>
<li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox" checked=""><font _mstmutation="1" _msttexthash="104179985" _msthash="306">可以访问文档数据库（小样本培训 / RAG）</font></li>
<li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox" checked=""><font _mstmutation="1" _msttexthash="75365212" _msthash="307">帮助用户查找完成索赔所需的信息</font></li>
<li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox" checked=""><font _mstmutation="1" _msttexthash="13132236" _msthash="308">越狱检测</font></li>
<li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox" checked=""><font _mstmutation="1" _msttexthash="78354952" _msthash="309">通过 usign a Redis 缓存降低 AI 搜索成本</font></li>
<li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox" checked=""><font _mstmutation="1" _msttexthash="94813875" _msthash="310">使用 Application Insights 进行监控和跟踪</font></li>
<li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox" checked=""><font _mstmutation="1" _msttexthash="55619863" _msthash="311">使用功能标志执行用户测试</font></li>
<li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox" checked=""><font _mstmutation="1" _msttexthash="77149475" _msthash="312">在对话期间接收 SMS 以获取明确措辞</font></li>
<li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox" checked=""><font _mstmutation="1" _msttexthash="60241870" _msthash="313">记录审计和质量保证的电话</font></li>
<li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox" checked=""><font _mstmutation="1" _msttexthash="142164386" _msthash="314">响应从 LLM 流式传输给用户，以避免长时间停顿</font></li>
<li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox" checked=""><font _mstmutation="1" _msttexthash="34708414" _msthash="315">通话后发送短信报告</font></li>
<li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox" checked=""><font _mstmutation="1" _msttexthash="35418916" _msthash="316">脱离会话后收回对话</font></li>
<li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox"><font _mstmutation="1" _msttexthash="25672153" _msthash="317">需要时回拨用户</font></li>
<li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox"><font _mstmutation="1" _msttexthash="23502089" _msthash="318">模拟 IVR 工作流程</font></li>
</ul>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto" _msttexthash="5815212" _msthash="319">演示</h3><a id="user-content-demo" class="anchor" aria-label="永久链接： Demo" href="#demo" _mstaria-label="241150" _msthash="320"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto" _msttexthash="405448862" _msthash="321">YouTube 上提供了法语演示。不要犹豫，以 x1.5 的速度观看演示，以快速了解该项目。</p>
<p dir="auto"><a href="https://youtube.com/watch?v=WvEVN5v8jW4" rel="nofollow"><img src="https://camo.githubusercontent.com/40399f81b43061b406bf6c5ce405e3423216270550a5887fde47cb86155e8bc7/68747470733a2f2f696d672e796f75747562652e636f6d2f76692f577645564e3576386a57342f6d617872657364656661756c742e6a7067" alt="法语演示" data-canonical-src="https://img.youtube.com/vi/WvEVN5v8jW4/maxresdefault.jpg" style="max-width: 100%;" _mstalt="154349" _msthash="322"></a></p>
<p dir="auto" _msttexthash="53063478" _msthash="323">演示中显示的主要交互：</p>
<ol dir="auto">
<li _msttexthash="17353609" _msthash="324">用户呼叫中心</li>
<li _msttexthash="38573821" _msthash="325">机器人回答并开始对话</li>
<li _msttexthash="109143086" _msthash="326">机器人将 conversation、claim 和 todo list 存储在数据库中</li>
</ol>
<p dir="auto" _msttexthash="61181692" _msthash="327">调用期间存储的数据提取：</p>
<div class="highlight highlight-source-json notranslate position-relative overflow-auto" dir="auto"><pre>{
  <span class="pl-ent">"claim"</span>: {
    <span class="pl-ent">"incident_datetime"</span>: <span class="pl-s"><span class="pl-pds">"</span>2024-10-08T02:00:00<span class="pl-pds">"</span></span>,
    <span class="pl-ent">"incident_description"</span>: <span class="pl-s"><span class="pl-pds">"</span>La trottinette électrique fait des bruits bizarres et émet de la fumée blanche.<span class="pl-pds">"</span></span>,
    <span class="pl-ent">"incident_location"</span>: <span class="pl-s"><span class="pl-pds">"</span>46 rue du Charles de Gaulle<span class="pl-pds">"</span></span>,
    <span class="pl-ent">"injuries"</span>: <span class="pl-s"><span class="pl-pds">"</span>Douleur au genou suite à une chute.<span class="pl-pds">"</span></span>,
    <span class="pl-ent">"involved_parties"</span>: <span class="pl-s"><span class="pl-pds">"</span>Lesne<span class="pl-pds">"</span></span>,
    <span class="pl-ent">"policy_number"</span>: <span class="pl-s"><span class="pl-pds">"</span>B02131325XPGOLMP<span class="pl-pds">"</span></span>
  },
  <span class="pl-ent">"messages"</span>: [
    {
      <span class="pl-ent">"created_at"</span>: <span class="pl-s"><span class="pl-pds">"</span>2024-10-08T11:23:41.824758Z<span class="pl-pds">"</span></span>,
      <span class="pl-ent">"action"</span>: <span class="pl-s"><span class="pl-pds">"</span>call<span class="pl-pds">"</span></span>,
      <span class="pl-ent">"content"</span>: <span class="pl-s"><span class="pl-pds">"</span><span class="pl-pds">"</span></span>,
      <span class="pl-ent">"persona"</span>: <span class="pl-s"><span class="pl-pds">"</span>human<span class="pl-pds">"</span></span>,
      <span class="pl-ent">"style"</span>: <span class="pl-s"><span class="pl-pds">"</span>none<span class="pl-pds">"</span></span>,
      <span class="pl-ent">"tool_calls"</span>: []
    },
    {
      <span class="pl-ent">"created_at"</span>: <span class="pl-s"><span class="pl-pds">"</span>2024-10-08T11:23:55.421654Z<span class="pl-pds">"</span></span>,
      <span class="pl-ent">"action"</span>: <span class="pl-s"><span class="pl-pds">"</span>talk<span class="pl-pds">"</span></span>,
      <span class="pl-ent">"content"</span>: <span class="pl-s"><span class="pl-pds">"</span>Bonjour, je m'appelle Amélie, de Contoso Assurance ! Comment puis-je vous aider aujourd'hui ?<span class="pl-pds">"</span></span>,
      <span class="pl-ent">"persona"</span>: <span class="pl-s"><span class="pl-pds">"</span>assistant<span class="pl-pds">"</span></span>,
      <span class="pl-ent">"style"</span>: <span class="pl-s"><span class="pl-pds">"</span>cheerful<span class="pl-pds">"</span></span>,
      <span class="pl-ent">"tool_calls"</span>: []
    },
    {
      <span class="pl-ent">"created_at"</span>: <span class="pl-s"><span class="pl-pds">"</span>2024-10-08T11:24:19.972737Z<span class="pl-pds">"</span></span>,
      <span class="pl-ent">"action"</span>: <span class="pl-s"><span class="pl-pds">"</span>talk<span class="pl-pds">"</span></span>,
      <span class="pl-ent">"content"</span>: <span class="pl-s"><span class="pl-pds">"</span>Oui bien sûr. Bonjour, je vous appelle parce que j'ai un problème avec ma trottinette électrique. Elle marche plus depuis ce matin, elle fait des bruits bizarres et il y a une fumée blanche qui sort de la trottinette.<span class="pl-pds">"</span></span>,
      <span class="pl-ent">"persona"</span>: <span class="pl-s"><span class="pl-pds">"</span>human<span class="pl-pds">"</span></span>,
      <span class="pl-ent">"style"</span>: <span class="pl-s"><span class="pl-pds">"</span>none<span class="pl-pds">"</span></span>,
      <span class="pl-ent">"tool_calls"</span>: []
    }
  ],
  <span class="pl-ent">"next"</span>: {
    <span class="pl-ent">"action"</span>: <span class="pl-s"><span class="pl-pds">"</span>case_closed<span class="pl-pds">"</span></span>,
    <span class="pl-ent">"justification"</span>: <span class="pl-s"><span class="pl-pds">"</span>The customer provided all necessary information for the claim, and they expressed satisfaction with the assistance received. No further action is required at this time.<span class="pl-pds">"</span></span>
  },
  <span class="pl-ent">"synthesis"</span>: {
    <span class="pl-ent">"long"</span>: <span class="pl-s"><span class="pl-pds">"</span>You reported an issue with your electric scooter, which started making strange noises and emitting white smoke. This incident occurred at 2:00 AM while you were riding it, leading to a fall and resulting in knee pain. The location of the incident was noted, and your policy details were confirmed. I have documented all the necessary information to file your claim. Please take care of your knee, and feel free to reach out if you need further assistance.<span class="pl-pds">"</span></span>,
    <span class="pl-ent">"satisfaction"</span>: <span class="pl-s"><span class="pl-pds">"</span>high<span class="pl-pds">"</span></span>,
    <span class="pl-ent">"short"</span>: <span class="pl-s"><span class="pl-pds">"</span>the breakdown of your scooter<span class="pl-pds">"</span></span>,
    <span class="pl-ent">"improvement_suggestions"</span>: <span class="pl-s"><span class="pl-pds">"</span>Ensure that the assistant provides clear next steps and offers to schedule follow-up calls proactively to enhance customer support.<span class="pl-pds">"</span></span>
  },
  <span class="pl-ii">...</span>
}</pre><div class="zeroclipboard-container">
    
  </div></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto" _msttexthash="29948633" _msthash="328">通话后的用户报告</h3><a id="user-content-user-report-after-the-call" class="anchor" aria-label="固定链接：通话后的用户报告" href="#user-report-after-the-call" _mstaria-label="984867" _msthash="329"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font _mstmutation="1" _msttexthash="178997910" _msthash="330">报告位于 （如 ）。它显示对话历史记录、索赔数据和提醒。</font><code>https://[your_domain]/report/[phone_number]</code><code>http://localhost:8080/report/%2B133658471534</code></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/microsoft/call-center-ai/blob/main/docs/user_report.png"><img src="/microsoft/call-center-ai/raw/main/docs/user_report.png" alt="用户报告" style="max-width: 100%;" _mstalt="163878" _msthash="331"></a></p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto" _msttexthash="13530582" _msthash="332">高级架构</h3><a id="user-content-high-level-architecture" class="anchor" aria-label="永久链接： 高级架构" href="#high-level-architecture" _mstaria-label="926601" _msthash="333"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<section class="js-render-needs-enrichment render-needs-enrichment position-relative" data-identity="23af2562-ae28-4569-9283-dc8c5bf20749" data-host="https://viewscreen.githubusercontent.com" data-src="https://viewscreen.githubusercontent.com/markdown/mermaid?docs_host=https%3A%2F%2Fdocs.github.com" data-type="mermaid" aria-label="Mermaid 渲染输出容器" _mstaria-label="906295" _msthash="334">
  <div class="js-render-enrichment-target" data-json="{&quot;data&quot;:&quot;---\ntitle: System diagram (C4 model)\n---\ngraph\n  user([\&quot;User\&quot;])\n  agent([\&quot;Agent\&quot;])\n\n  app[\&quot;Call Center AI\&quot;]\n\n  app -- Transfer to --&amp;gt; agent\n  app -. Send voice .-&amp;gt; user\n  user -- Call --&amp;gt; app\n&quot;}" data-plain="---
title: System diagram (C4 model)
---
graph
  user([&quot;User&quot;])
  agent([&quot;Agent&quot;])

  app[&quot;Call Center AI&quot;]

  app -- Transfer to --> agent
  app -. Send voice .-> user
  user -- Call --> app
" dir="auto"><!----><!----><div class="position-absolute top-0 pr-2 right-0 d-flex flex-justify-end flex-items-center">
    
    <details class="details-reset details-overlay details-overlay-dark" style="display: contents">
      <summary role="button" aria-label="“打开”对话框" class="btn my-2 mr-2 p-0 d-inline-flex" aria-haspopup="dialog" _mstaria-label="154752" _msthash="335">
        <svg width="16" height="16" viewBox="0 0 16 16" fill="currentColor" class="octicon m-2">
          <path fill-rule="evenodd" d="M3.72 3.72a.75.75 0 011.06 1.06L2.56 7h10.88l-2.22-2.22a.75.75 0 011.06-1.06l3.5 3.5a.75.75 0 010 1.06l-3.5 3.5a.75.75 0 11-1.06-1.06l2.22-2.22H2.56l2.22 2.22a.75.75 0 11-1.06 1.06l-3.5-3.5a.75.75 0 010-1.06l3.5-3.5z"></path>
        </svg>
      </summary>
      <details-dialog class="Box Box--overlay render-full-screen d-flex flex-column anim-fade-in fast" aria-label="mermaid rendered container" role="dialog" aria-modal="true" _msthidden="1" _mstaria-label="611598" _msthash="336">
        <div _msthidden="1">
          <button aria-label="Close dialog" data-close-dialog="" type="button" data-view-component="true" class="Link--muted btn-link position-absolute render-full-screen-close" _msthidden="A" _mstaria-label="177619" _msthash="337">
            <svg width="24" height="24" viewBox="0 0 24 24" fill="currentColor" style="display:inline-block;vertical-align:text-bottom" class="octicon octicon-x">
              <path fill-rule="evenodd" d="M5.72 5.72a.75.75 0 011.06 0L12 10.94l5.22-5.22a.75.75 0 111.06 1.06L13.06 12l5.22 5.22a.75.75 0 11-1.06 1.06L12 13.06l-5.22 5.22a.75.75 0 01-1.06-1.06L10.94 12 5.72 6.78a.75.75 0 010-1.06z"></path>
            </svg>
          </button>
          <div class="Box-body border-0" role="presentation"></div>
        </div>
      </details-dialog>
    </details>
  <!----> 
  </div><!---->
    <div class="render-container color-bg-transparent js-render-target p-0 is-render-automatic is-render-requested is-render-ready" data-identity="23af2562-ae28-4569-9283-dc8c5bf20749" data-host="https://viewscreen.githubusercontent.com" data-type="mermaid" style="height: 425.667px;">
      <iframe title="File display" role="presentation" class="render-viewer" sandbox="allow-scripts allow-same-origin allow-top-navigation allow-popups" src="https://viewscreen.githubusercontent.com/markdown/mermaid?docs_host=https%3A%2F%2Fdocs.github.com&amp;color_mode=light#23af2562-ae28-4569-9283-dc8c5bf20749" name="23af2562-ae28-4569-9283-dc8c5bf20749" data-content="{&quot;data&quot;:&quot;---\ntitle: System diagram (C4 model)\n---\ngraph\n  user([\&quot;User\&quot;])\n  agent([\&quot;Agent\&quot;])\n\n  app[\&quot;Call Center AI\&quot;]\n\n  app -- Transfer to --&amp;gt; agent\n  app -. Send voice .-&amp;gt; user\n  user -- Call --&amp;gt; app\n&quot;}">
      </iframe>
    </div>
  <!----><!----></div>
  <span class="js-render-enrichment-loader d-flex flex-justify-center flex-items-center width-full" style="min-height:100px" role="presentation" hidden="">
    <span data-view-component="true">
  <svg style="box-sizing: content-box; color: var(--color-icon-primary);" width="16" height="16" viewBox="0 0 16 16" fill="none" aria-hidden="true" data-view-component="true" class="octospinner mx-auto anim-rotate">
    <circle cx="8" cy="8" r="7" stroke="currentColor" stroke-opacity="0.25" stroke-width="2" vector-effect="non-scaling-stroke" fill="none"></circle>
    <path d="M15 8a7.002 7.002 0 00-7-7" stroke="currentColor" stroke-width="2" stroke-linecap="round" vector-effect="non-scaling-stroke"></path>
</svg>    <span class="sr-only" _msttexthash="92391" _msthash="339">Loading</span>
</span>
  </span>
<div class="js-render-enrichment-fallback" _msthidden="1"><div class="render-plaintext-hidden" dir="auto" _msthidden="1">
      <pre lang="mermaid" aria-label="Raw mermaid code" _msthidden="A" _mstaria-label="254033" _msthash="340">---
title: System diagram (C4 model)
---
graph
  user(["User"])
  agent(["Agent"])

  app["Call Center AI"]

  app -- Transfer to --&gt; agent
  app -. Send voice .-&gt; user
  user -- Call --&gt; app
</pre>
    </div></div></section>

<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto" _msttexthash="16089879" _msthash="341">组件级架构</h3><a id="user-content-component-level-architecture" class="anchor" aria-label="永久链接：组件级架构" href="#component-level-architecture" _mstaria-label="1212679" _msthash="342"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<section class="js-render-needs-enrichment render-needs-enrichment position-relative" data-identity="27487e82-f6d6-4b8a-926f-6b1e5681ec7a" data-host="https://viewscreen.githubusercontent.com" data-src="https://viewscreen.githubusercontent.com/markdown/mermaid?docs_host=https%3A%2F%2Fdocs.github.com" data-type="mermaid" aria-label="Mermaid 渲染输出容器" _mstaria-label="906295" _msthash="343">
  <div class="js-render-enrichment-target" data-json="{&quot;data&quot;:&quot;---\ntitle: Claim AI component diagram (C4 model)\n---\ngraph LR\n  agent([\&quot;Agent\&quot;])\n  user([\&quot;User\&quot;])\n\n  subgraph \&quot;Claim AI\&quot;\n    ada[\&quot;Embedding&amp;lt;br&amp;gt;(ADA)\&quot;]\n    app[\&quot;App&amp;lt;br&amp;gt;(Container App)\&quot;]\n    communication_services[\&quot;Call &amp;amp; SMS gateway&amp;lt;br&amp;gt;(Communication Services)\&quot;]\n    db[(\&quot;Conversations and claims&amp;lt;br&amp;gt;(Cosmos DB / SQLite)\&quot;)]\n    eventgrid[\&quot;Broker&amp;lt;br&amp;gt;(Event Grid)\&quot;]\n    gpt[\&quot;LLM&amp;lt;br&amp;gt;(GPT-4o)\&quot;]\n    queues[(\&quot;Queues&amp;lt;br&amp;gt;(Azure Storage)\&quot;)]\n    redis[(\&quot;Cache&amp;lt;br&amp;gt;(Redis)\&quot;)]\n    search[(\&quot;RAG&amp;lt;br&amp;gt;(AI Search)\&quot;)]\n    sounds[(\&quot;Sounds&amp;lt;br&amp;gt;(Azure Storage)\&quot;)]\n    sst[\&quot;Speech-to-Text&amp;lt;br&amp;gt;(Cognitive Services)\&quot;]\n    translation[\&quot;Translation&amp;lt;br&amp;gt;(Cognitive Services)\&quot;]\n    tts[\&quot;Text-to-Speech&amp;lt;br&amp;gt;(Cognitive Services)\&quot;]\n  end\n\n  app -- Respond with text --&amp;gt; communication_services\n  app -- Ask for translation --&amp;gt; translation\n  app -- Ask to transfer --&amp;gt; communication_services\n  app -- Few-shot training --&amp;gt; search\n  app -- Generate completion --&amp;gt; gpt\n  app -- Get cached data --&amp;gt; redis\n  app -- Save conversation --&amp;gt; db\n  app -- Send SMS report --&amp;gt; communication_services\n  app -. Watch .-&amp;gt; queues\n\n  communication_services -- Generate voice --&amp;gt; tts\n  communication_services -- Load sound --&amp;gt; sounds\n  communication_services -- Notifies --&amp;gt; eventgrid\n  communication_services -- Send SMS --&amp;gt; user\n  communication_services -- Transfer to --&amp;gt; agent\n  communication_services -- Transform voice --&amp;gt; sst\n  communication_services -. Send voice .-&amp;gt; user\n\n  eventgrid -- Push to --&amp;gt; queues\n\n  search -- Generate embeddings --&amp;gt; ada\n\n  user -- Call --&amp;gt; communication_services\n&quot;}" data-plain="---
title: Claim AI component diagram (C4 model)
---
graph LR
  agent([&quot;Agent&quot;])
  user([&quot;User&quot;])

  subgraph &quot;Claim AI&quot;
    ada[&quot;Embedding<br>(ADA)&quot;]
    app[&quot;App<br>(Container App)&quot;]
    communication_services[&quot;Call &amp; SMS gateway<br>(Communication Services)&quot;]
    db[(&quot;Conversations and claims<br>(Cosmos DB / SQLite)&quot;)]
    eventgrid[&quot;Broker<br>(Event Grid)&quot;]
    gpt[&quot;LLM<br>(GPT-4o)&quot;]
    queues[(&quot;Queues<br>(Azure Storage)&quot;)]
    redis[(&quot;Cache<br>(Redis)&quot;)]
    search[(&quot;RAG<br>(AI Search)&quot;)]
    sounds[(&quot;Sounds<br>(Azure Storage)&quot;)]
    sst[&quot;Speech-to-Text<br>(Cognitive Services)&quot;]
    translation[&quot;Translation<br>(Cognitive Services)&quot;]
    tts[&quot;Text-to-Speech<br>(Cognitive Services)&quot;]
  end

  app -- Respond with text --> communication_services
  app -- Ask for translation --> translation
  app -- Ask to transfer --> communication_services
  app -- Few-shot training --> search
  app -- Generate completion --> gpt
  app -- Get cached data --> redis
  app -- Save conversation --> db
  app -- Send SMS report --> communication_services
  app -. Watch .-> queues

  communication_services -- Generate voice --> tts
  communication_services -- Load sound --> sounds
  communication_services -- Notifies --> eventgrid
  communication_services -- Send SMS --> user
  communication_services -- Transfer to --> agent
  communication_services -- Transform voice --> sst
  communication_services -. Send voice .-> user

  eventgrid -- Push to --> queues

  search -- Generate embeddings --> ada

  user -- Call --> communication_services
" dir="auto"><!----><!----><div class="position-absolute top-0 pr-2 right-0 d-flex flex-justify-end flex-items-center">
    
    <details class="details-reset details-overlay details-overlay-dark" style="display: contents">
      <summary role="button" aria-label="“打开”对话框" class="btn my-2 mr-2 p-0 d-inline-flex" aria-haspopup="dialog" _mstaria-label="154752" _msthash="344">
        <svg width="16" height="16" viewBox="0 0 16 16" fill="currentColor" class="octicon m-2">
          <path fill-rule="evenodd" d="M3.72 3.72a.75.75 0 011.06 1.06L2.56 7h10.88l-2.22-2.22a.75.75 0 011.06-1.06l3.5 3.5a.75.75 0 010 1.06l-3.5 3.5a.75.75 0 11-1.06-1.06l2.22-2.22H2.56l2.22 2.22a.75.75 0 11-1.06 1.06l-3.5-3.5a.75.75 0 010-1.06l3.5-3.5z"></path>
        </svg>
      </summary>
      <details-dialog class="Box Box--overlay render-full-screen d-flex flex-column anim-fade-in fast" aria-label="mermaid rendered container" role="dialog" aria-modal="true" _msthidden="1" _mstaria-label="611598" _msthash="345">
        <div _msthidden="1">
          <button aria-label="Close dialog" data-close-dialog="" type="button" data-view-component="true" class="Link--muted btn-link position-absolute render-full-screen-close" _msthidden="A" _mstaria-label="177619" _msthash="346">
            <svg width="24" height="24" viewBox="0 0 24 24" fill="currentColor" style="display:inline-block;vertical-align:text-bottom" class="octicon octicon-x">
              <path fill-rule="evenodd" d="M5.72 5.72a.75.75 0 011.06 0L12 10.94l5.22-5.22a.75.75 0 111.06 1.06L13.06 12l5.22 5.22a.75.75 0 11-1.06 1.06L12 13.06l-5.22 5.22a.75.75 0 01-1.06-1.06L10.94 12 5.72 6.78a.75.75 0 010-1.06z"></path>
            </svg>
          </button>
          <div class="Box-body border-0" role="presentation"></div>
        </div>
      </details-dialog>
    </details>
  <!----> 
  </div><!---->
    <div class="render-container color-bg-transparent js-render-target p-0 is-render-automatic is-render-requested is-render-ready" data-identity="27487e82-f6d6-4b8a-926f-6b1e5681ec7a" data-host="https://viewscreen.githubusercontent.com" data-type="mermaid" style="height: 802.105px;">
      <iframe title="File display" role="presentation" class="render-viewer" sandbox="allow-scripts allow-same-origin allow-top-navigation allow-popups" src="https://viewscreen.githubusercontent.com/markdown/mermaid?docs_host=https%3A%2F%2Fdocs.github.com&amp;color_mode=light#27487e82-f6d6-4b8a-926f-6b1e5681ec7a" name="27487e82-f6d6-4b8a-926f-6b1e5681ec7a" data-content="{&quot;data&quot;:&quot;---\ntitle: Claim AI component diagram (C4 model)\n---\ngraph LR\n  agent([\&quot;Agent\&quot;])\n  user([\&quot;User\&quot;])\n\n  subgraph \&quot;Claim AI\&quot;\n    ada[\&quot;Embedding&amp;lt;br&amp;gt;(ADA)\&quot;]\n    app[\&quot;App&amp;lt;br&amp;gt;(Container App)\&quot;]\n    communication_services[\&quot;Call &amp;amp; SMS gateway&amp;lt;br&amp;gt;(Communication Services)\&quot;]\n    db[(\&quot;Conversations and claims&amp;lt;br&amp;gt;(Cosmos DB / SQLite)\&quot;)]\n    eventgrid[\&quot;Broker&amp;lt;br&amp;gt;(Event Grid)\&quot;]\n    gpt[\&quot;LLM&amp;lt;br&amp;gt;(GPT-4o)\&quot;]\n    queues[(\&quot;Queues&amp;lt;br&amp;gt;(Azure Storage)\&quot;)]\n    redis[(\&quot;Cache&amp;lt;br&amp;gt;(Redis)\&quot;)]\n    search[(\&quot;RAG&amp;lt;br&amp;gt;(AI Search)\&quot;)]\n    sounds[(\&quot;Sounds&amp;lt;br&amp;gt;(Azure Storage)\&quot;)]\n    sst[\&quot;Speech-to-Text&amp;lt;br&amp;gt;(Cognitive Services)\&quot;]\n    translation[\&quot;Translation&amp;lt;br&amp;gt;(Cognitive Services)\&quot;]\n    tts[\&quot;Text-to-Speech&amp;lt;br&amp;gt;(Cognitive Services)\&quot;]\n  end\n\n  app -- Respond with text --&amp;gt; communication_services\n  app -- Ask for translation --&amp;gt; translation\n  app -- Ask to transfer --&amp;gt; communication_services\n  app -- Few-shot training --&amp;gt; search\n  app -- Generate completion --&amp;gt; gpt\n  app -- Get cached data --&amp;gt; redis\n  app -- Save conversation --&amp;gt; db\n  app -- Send SMS report --&amp;gt; communication_services\n  app -. Watch .-&amp;gt; queues\n\n  communication_services -- Generate voice --&amp;gt; tts\n  communication_services -- Load sound --&amp;gt; sounds\n  communication_services -- Notifies --&amp;gt; eventgrid\n  communication_services -- Send SMS --&amp;gt; user\n  communication_services -- Transfer to --&amp;gt; agent\n  communication_services -- Transform voice --&amp;gt; sst\n  communication_services -. Send voice .-&amp;gt; user\n\n  eventgrid -- Push to --&amp;gt; queues\n\n  search -- Generate embeddings --&amp;gt; ada\n\n  user -- Call --&amp;gt; communication_services\n&quot;}">
      </iframe>
    </div>
  <!----><!----></div>
  <span class="js-render-enrichment-loader d-flex flex-justify-center flex-items-center width-full" style="min-height:100px" role="presentation" hidden="">
    <span data-view-component="true">
  <svg style="box-sizing: content-box; color: var(--color-icon-primary);" width="16" height="16" viewBox="0 0 16 16" fill="none" aria-hidden="true" data-view-component="true" class="octospinner mx-auto anim-rotate">
    <circle cx="8" cy="8" r="7" stroke="currentColor" stroke-opacity="0.25" stroke-width="2" vector-effect="non-scaling-stroke" fill="none"></circle>
    <path d="M15 8a7.002 7.002 0 00-7-7" stroke="currentColor" stroke-width="2" stroke-linecap="round" vector-effect="non-scaling-stroke"></path>
</svg>    <span class="sr-only" _msttexthash="92391" _msthash="348">Loading</span>
</span>
  </span>
<div class="js-render-enrichment-fallback" _msthidden="1"><div class="render-plaintext-hidden" dir="auto" _msthidden="1">
      <pre lang="mermaid" aria-label="Raw mermaid code" _msthidden="A" _mstaria-label="254033" _msthash="349">---
title: Claim AI component diagram (C4 model)
---
graph LR
  agent(["Agent"])
  user(["User"])

  subgraph "Claim AI"
    ada["Embedding&lt;br&gt;(ADA)"]
    app["App&lt;br&gt;(Container App)"]
    communication_services["Call &amp; SMS gateway&lt;br&gt;(Communication Services)"]
    db[("Conversations and claims&lt;br&gt;(Cosmos DB / SQLite)")]
    eventgrid["Broker&lt;br&gt;(Event Grid)"]
    gpt["LLM&lt;br&gt;(GPT-4o)"]
    queues[("Queues&lt;br&gt;(Azure Storage)")]
    redis[("Cache&lt;br&gt;(Redis)")]
    search[("RAG&lt;br&gt;(AI Search)")]
    sounds[("Sounds&lt;br&gt;(Azure Storage)")]
    sst["Speech-to-Text&lt;br&gt;(Cognitive Services)"]
    translation["Translation&lt;br&gt;(Cognitive Services)"]
    tts["Text-to-Speech&lt;br&gt;(Cognitive Services)"]
  end

  app -- Respond with text --&gt; communication_services
  app -- Ask for translation --&gt; translation
  app -- Ask to transfer --&gt; communication_services
  app -- Few-shot training --&gt; search
  app -- Generate completion --&gt; gpt
  app -- Get cached data --&gt; redis
  app -- Save conversation --&gt; db
  app -- Send SMS report --&gt; communication_services
  app -. Watch .-&gt; queues

  communication_services -- Generate voice --&gt; tts
  communication_services -- Load sound --&gt; sounds
  communication_services -- Notifies --&gt; eventgrid
  communication_services -- Send SMS --&gt; user
  communication_services -- Transfer to --&gt; agent
  communication_services -- Transform voice --&gt; sst
  communication_services -. Send voice .-&gt; user

  eventgrid -- Push to --&gt; queues

  search -- Generate embeddings --&gt; ada

  user -- Call --&gt; communication_services
</pre>
    </div></div></section>

<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto" _msttexthash="6993987" _msthash="350">序列图</h3><a id="user-content-sequence-diagram" class="anchor" aria-label="永久链接：序列图" href="#sequence-diagram" _mstaria-label="631423" _msthash="351"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<section class="js-render-needs-enrichment render-needs-enrichment position-relative" data-identity="df9b02ec-4ae5-4580-97eb-9b61f67b96de" data-host="https://viewscreen.githubusercontent.com" data-src="https://viewscreen.githubusercontent.com/markdown/mermaid?docs_host=https%3A%2F%2Fdocs.github.com" data-type="mermaid" aria-label="Mermaid 渲染输出容器" _mstaria-label="906295" _msthash="352">
  <div class="js-render-enrichment-target" data-json="{&quot;data&quot;:&quot;sequenceDiagram\n    autonumber\n\n    actor Customer\n    participant PSTN\n    participant Text to Speech\n    participant Speech to Text\n    actor Human agent\n    participant Event Grid\n    participant Communication Services\n    participant App\n    participant Cosmos DB\n    participant OpenAI GPT\n    participant AI Search\n\n    App-&amp;gt;&amp;gt;Event Grid: Subscribe to events\n    Customer-&amp;gt;&amp;gt;PSTN: Initiate a call\n    PSTN-&amp;gt;&amp;gt;Communication Services: Forward call\n    Communication Services-&amp;gt;&amp;gt;Event Grid: New call event\n    Event Grid-&amp;gt;&amp;gt;App: Send event to event URL (HTTP webhook)\n    activate App\n    App-&amp;gt;&amp;gt;Communication Services: Accept the call and give inbound URL\n    deactivate App\n    Communication Services-&amp;gt;&amp;gt;Speech to Text: Transform speech to text\n\n    Communication Services-&amp;gt;&amp;gt;App: Send text to the inbound URL\n    activate App\n    alt First call\n        App-&amp;gt;&amp;gt;Communication Services: Send static SSML text\n    else Callback\n        App-&amp;gt;&amp;gt;AI Search: Gather training data\n        App-&amp;gt;&amp;gt;OpenAI GPT: Ask for a completion\n        OpenAI GPT--&amp;gt;&amp;gt;App: Respond (HTTP/2 SSE)\n        loop Over buffer\n            loop Over multiple tools\n                alt Is this a claim data update?\n                    App-&amp;gt;&amp;gt;Cosmos DB: Update claim data\n                else Does the user want the human agent?\n                    App-&amp;gt;&amp;gt;Communication Services: Send static SSML text\n                    App-&amp;gt;&amp;gt;Communication Services: Transfer to a human\n                    Communication Services-&amp;gt;&amp;gt;Human agent: Call the phone number\n                else Should we end the call?\n                    App-&amp;gt;&amp;gt;Communication Services: Send static SSML text\n                    App-&amp;gt;&amp;gt;Communication Services: End the call\n                end\n            end\n        end\n        App-&amp;gt;&amp;gt;Cosmos DB: Persist conversation\n    end\n    deactivate App\n    Communication Services-&amp;gt;&amp;gt;PSTN: Send voice\n    PSTN-&amp;gt;&amp;gt;Customer: Forward voice\n&quot;}" data-plain="sequenceDiagram
    autonumber

    actor Customer
    participant PSTN
    participant Text to Speech
    participant Speech to Text
    actor Human agent
    participant Event Grid
    participant Communication Services
    participant App
    participant Cosmos DB
    participant OpenAI GPT
    participant AI Search

    App->>Event Grid: Subscribe to events
    Customer->>PSTN: Initiate a call
    PSTN->>Communication Services: Forward call
    Communication Services->>Event Grid: New call event
    Event Grid->>App: Send event to event URL (HTTP webhook)
    activate App
    App->>Communication Services: Accept the call and give inbound URL
    deactivate App
    Communication Services->>Speech to Text: Transform speech to text

    Communication Services->>App: Send text to the inbound URL
    activate App
    alt First call
        App->>Communication Services: Send static SSML text
    else Callback
        App->>AI Search: Gather training data
        App->>OpenAI GPT: Ask for a completion
        OpenAI GPT-->>App: Respond (HTTP/2 SSE)
        loop Over buffer
            loop Over multiple tools
                alt Is this a claim data update?
                    App->>Cosmos DB: Update claim data
                else Does the user want the human agent?
                    App->>Communication Services: Send static SSML text
                    App->>Communication Services: Transfer to a human
                    Communication Services->>Human agent: Call the phone number
                else Should we end the call?
                    App->>Communication Services: Send static SSML text
                    App->>Communication Services: End the call
                end
            end
        end
        App->>Cosmos DB: Persist conversation
    end
    deactivate App
    Communication Services->>PSTN: Send voice
    PSTN->>Customer: Forward voice
" dir="auto"><!----><!----><div class="position-absolute top-0 pr-2 right-0 d-flex flex-justify-end flex-items-center">
    
    <details class="details-reset details-overlay details-overlay-dark" style="display: contents">
      <summary role="button" aria-label="“打开”对话框" class="btn my-2 mr-2 p-0 d-inline-flex" aria-haspopup="dialog" _mstaria-label="154752" _msthash="353">
        <svg width="16" height="16" viewBox="0 0 16 16" fill="currentColor" class="octicon m-2">
          <path fill-rule="evenodd" d="M3.72 3.72a.75.75 0 011.06 1.06L2.56 7h10.88l-2.22-2.22a.75.75 0 011.06-1.06l3.5 3.5a.75.75 0 010 1.06l-3.5 3.5a.75.75 0 11-1.06-1.06l2.22-2.22H2.56l2.22 2.22a.75.75 0 11-1.06 1.06l-3.5-3.5a.75.75 0 010-1.06l3.5-3.5z"></path>
        </svg>
      </summary>
      <details-dialog class="Box Box--overlay render-full-screen d-flex flex-column anim-fade-in fast" aria-label="mermaid rendered container" role="dialog" aria-modal="true" _msthidden="1" _mstaria-label="611598" _msthash="354">
        <div _msthidden="1">
          <button aria-label="Close dialog" data-close-dialog="" type="button" data-view-component="true" class="Link--muted btn-link position-absolute render-full-screen-close" _msthidden="A" _mstaria-label="177619" _msthash="355">
            <svg width="24" height="24" viewBox="0 0 24 24" fill="currentColor" style="display:inline-block;vertical-align:text-bottom" class="octicon octicon-x">
              <path fill-rule="evenodd" d="M5.72 5.72a.75.75 0 011.06 0L12 10.94l5.22-5.22a.75.75 0 111.06 1.06L13.06 12l5.22 5.22a.75.75 0 11-1.06 1.06L12 13.06l-5.22 5.22a.75.75 0 01-1.06-1.06L10.94 12 5.72 6.78a.75.75 0 010-1.06z"></path>
            </svg>
          </button>
          <div class="Box-body border-0" role="presentation"></div>
        </div>
      </details-dialog>
    </details>
  <!----> 
  </div><!---->
    <div class="render-container color-bg-transparent js-render-target p-0 is-render-automatic is-render-requested is-render-ready" data-identity="df9b02ec-4ae5-4580-97eb-9b61f67b96de" data-host="https://viewscreen.githubusercontent.com" data-type="mermaid" style="height: 551.133px;">
      <iframe title="File display" role="presentation" class="render-viewer" sandbox="allow-scripts allow-same-origin allow-top-navigation allow-popups" src="https://viewscreen.githubusercontent.com/markdown/mermaid?docs_host=https%3A%2F%2Fdocs.github.com&amp;color_mode=light#df9b02ec-4ae5-4580-97eb-9b61f67b96de" name="df9b02ec-4ae5-4580-97eb-9b61f67b96de" data-content="{&quot;data&quot;:&quot;sequenceDiagram\n    autonumber\n\n    actor Customer\n    participant PSTN\n    participant Text to Speech\n    participant Speech to Text\n    actor Human agent\n    participant Event Grid\n    participant Communication Services\n    participant App\n    participant Cosmos DB\n    participant OpenAI GPT\n    participant AI Search\n\n    App-&amp;gt;&amp;gt;Event Grid: Subscribe to events\n    Customer-&amp;gt;&amp;gt;PSTN: Initiate a call\n    PSTN-&amp;gt;&amp;gt;Communication Services: Forward call\n    Communication Services-&amp;gt;&amp;gt;Event Grid: New call event\n    Event Grid-&amp;gt;&amp;gt;App: Send event to event URL (HTTP webhook)\n    activate App\n    App-&amp;gt;&amp;gt;Communication Services: Accept the call and give inbound URL\n    deactivate App\n    Communication Services-&amp;gt;&amp;gt;Speech to Text: Transform speech to text\n\n    Communication Services-&amp;gt;&amp;gt;App: Send text to the inbound URL\n    activate App\n    alt First call\n        App-&amp;gt;&amp;gt;Communication Services: Send static SSML text\n    else Callback\n        App-&amp;gt;&amp;gt;AI Search: Gather training data\n        App-&amp;gt;&amp;gt;OpenAI GPT: Ask for a completion\n        OpenAI GPT--&amp;gt;&amp;gt;App: Respond (HTTP/2 SSE)\n        loop Over buffer\n            loop Over multiple tools\n                alt Is this a claim data update?\n                    App-&amp;gt;&amp;gt;Cosmos DB: Update claim data\n                else Does the user want the human agent?\n                    App-&amp;gt;&amp;gt;Communication Services: Send static SSML text\n                    App-&amp;gt;&amp;gt;Communication Services: Transfer to a human\n                    Communication Services-&amp;gt;&amp;gt;Human agent: Call the phone number\n                else Should we end the call?\n                    App-&amp;gt;&amp;gt;Communication Services: Send static SSML text\n                    App-&amp;gt;&amp;gt;Communication Services: End the call\n                end\n            end\n        end\n        App-&amp;gt;&amp;gt;Cosmos DB: Persist conversation\n    end\n    deactivate App\n    Communication Services-&amp;gt;&amp;gt;PSTN: Send voice\n    PSTN-&amp;gt;&amp;gt;Customer: Forward voice\n&quot;}">
      </iframe>
    </div>
  <!----><!----></div>
  <span class="js-render-enrichment-loader d-flex flex-justify-center flex-items-center width-full" style="min-height:100px" role="presentation" hidden="">
    <span data-view-component="true">
  <svg style="box-sizing: content-box; color: var(--color-icon-primary);" width="16" height="16" viewBox="0 0 16 16" fill="none" aria-hidden="true" data-view-component="true" class="octospinner mx-auto anim-rotate">
    <circle cx="8" cy="8" r="7" stroke="currentColor" stroke-opacity="0.25" stroke-width="2" vector-effect="non-scaling-stroke" fill="none"></circle>
    <path d="M15 8a7.002 7.002 0 00-7-7" stroke="currentColor" stroke-width="2" stroke-linecap="round" vector-effect="non-scaling-stroke"></path>
</svg>    <span class="sr-only" _msttexthash="92391" _msthash="357">Loading</span>
</span>
  </span>
<div class="js-render-enrichment-fallback" _msthidden="1"><div class="render-plaintext-hidden" dir="auto" _msthidden="1">
      <pre lang="mermaid" aria-label="Raw mermaid code" _msthidden="A" _mstaria-label="254033" _msthash="358">sequenceDiagram
    autonumber

    actor Customer
    participant PSTN
    participant Text to Speech
    participant Speech to Text
    actor Human agent
    participant Event Grid
    participant Communication Services
    participant App
    participant Cosmos DB
    participant OpenAI GPT
    participant AI Search

    App-&gt;&gt;Event Grid: Subscribe to events
    Customer-&gt;&gt;PSTN: Initiate a call
    PSTN-&gt;&gt;Communication Services: Forward call
    Communication Services-&gt;&gt;Event Grid: New call event
    Event Grid-&gt;&gt;App: Send event to event URL (HTTP webhook)
    activate App
    App-&gt;&gt;Communication Services: Accept the call and give inbound URL
    deactivate App
    Communication Services-&gt;&gt;Speech to Text: Transform speech to text

    Communication Services-&gt;&gt;App: Send text to the inbound URL
    activate App
    alt First call
        App-&gt;&gt;Communication Services: Send static SSML text
    else Callback
        App-&gt;&gt;AI Search: Gather training data
        App-&gt;&gt;OpenAI GPT: Ask for a completion
        OpenAI GPT--&gt;&gt;App: Respond (HTTP/2 SSE)
        loop Over buffer
            loop Over multiple tools
                alt Is this a claim data update?
                    App-&gt;&gt;Cosmos DB: Update claim data
                else Does the user want the human agent?
                    App-&gt;&gt;Communication Services: Send static SSML text
                    App-&gt;&gt;Communication Services: Transfer to a human
                    Communication Services-&gt;&gt;Human agent: Call the phone number
                else Should we end the call?
                    App-&gt;&gt;Communication Services: Send static SSML text
                    App-&gt;&gt;Communication Services: End the call
                end
            end
        end
        App-&gt;&gt;Cosmos DB: Persist conversation
    end
    deactivate App
    Communication Services-&gt;&gt;PSTN: Send voice
    PSTN-&gt;&gt;Customer: Forward voice
</pre>
    </div></div></section>

<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto" _msttexthash="6768840" _msthash="359">部署</h2><a id="user-content-deployment" class="anchor" aria-label="永久链接：部署" href="#deployment" _mstaria-label="445081" _msthash="360"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto" _msttexthash="9792913" _msthash="361">先决条件</h3><a id="user-content-prerequisites" class="anchor" aria-label="永久链接：先决条件" href="#prerequisites" _mstaria-label="566982" _msthash="362"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto" _msttexthash="298663729" _msthash="363"><a href="https://codespaces.new/microsoft/call-center-ai?quickstart=1" rel="nofollow" _istranslated="1">首选使用 GitHub Codespaces 快速入门。</a>环境将使用所有必需的工具自动设置。</p>
<p dir="auto"><font _mstmutation="1" _msttexthash="102489478" _msthash="364">在 macOS 中，使用 <a href="https://brew.sh" rel="nofollow" _mstmutation="1" _istranslated="1">Homebrew</a> 时，只需键入 .</font><code>make brew</code></p>
<p dir="auto" _msttexthash="110276517" _msthash="365">对于其他系统，请确保已安装以下内容：</p>
<ul dir="auto">
<li><font _mstmutation="1" _msttexthash="51325365" _msthash="366">与 Bash 兼容的 shell，例如 或</font><code>bash</code><code>zsh</code></li>
<li><a href="https://github.com/mikefarah/yq?tab=readme-ov-file#install" _msttexthash="16523" _msthash="367">YQ</a></li>
<li><font _mstmutation="1" _msttexthash="127841285" _msthash="368">品牌、（Ubuntu）、（CentOS）、（macOS）</font><code>apt install make</code><code>yum install make</code><code>brew install make</code></li>
<li><a href="https://learn.microsoft.com/en-us/cli/azure/install-azure-cli" rel="nofollow" _msttexthash="98137" _msthash="369">Azure CLI</a></li>
<li><a href="https://github.com/Azure/azure-functions-core-tools?tab=readme-ov-file#installing" _msttexthash="15238600" _msthash="370">Azure Functions Core 工具</a></li>
<li _msttexthash="43201262" _msthash="371"><a href="https://www.twilio.com/docs/twilio-cli/getting-started/install" rel="nofollow" _istranslated="1">Twilio CLI</a>（可选）</li>
</ul>
<p dir="auto" _msttexthash="53414673" _msthash="372">然后，需要 Azure 资源：</p>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto" _msttexthash="31676086" _msthash="373">1. <a href="https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/manage-resource-groups-portal" rel="nofollow" _istranslated="1">创建新的资源组</a></h4><a id="user-content-1-create-a-new-resource-group" class="anchor" aria-label="永久链接：1. 创建新的资源组" href="#1-create-a-new-resource-group" _mstaria-label="1133925" _msthash="374"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ul dir="auto">
<li><font _mstmutation="1" _msttexthash="200499052" _msthash="375">喜欢使用小写字母，并且不使用短划线以外的特殊字符（例如</font><code>ccai-customer-a</code>)</li>
</ul>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto" _msttexthash="35342138" _msthash="376">2. <a href="https://learn.microsoft.com/en-us/azure/communication-services/quickstarts/create-communication-resource?tabs=linux&amp;pivots=platform-azp" rel="nofollow" _istranslated="1">创建通信服务资源</a></h4><a id="user-content-2-create-a-communication-services-resource" class="anchor" aria-label="永久链接：2. 创建通信服务资源" href="#2-create-a-communication-services-resource" _mstaria-label="1973556" _msthash="377"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ul dir="auto">
<li _msttexthash="19543186" _msthash="378">与资源组同名</li>
<li _msttexthash="32596369" _msthash="379">启用系统托管标识</li>
</ul>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto" _msttexthash="25948494" _msthash="380">3. <a href="https://learn.microsoft.com/en-us/azure/communication-services/quickstarts/telephony/get-phone-number?tabs=linux&amp;pivots=platform-azp-new" rel="nofollow" _istranslated="1">购买电话号码</a></h4><a id="user-content-3-buy-a-phone-number" class="anchor" aria-label="永久链接：3. 购买电话号码" href="#3-buy-a-phone-number" _mstaria-label="707954" _msthash="381"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ul dir="auto">
<li _msttexthash="24944296" _msthash="382">从通信服务资源</li>
<li _msttexthash="34524386" _msthash="383">允许入站和出站通信</li>
<li _msttexthash="124948174" _msthash="384">启用语音（必需）和短信（可选）功能</li>
</ul>
<p dir="auto" _msttexthash="185138772" _msthash="385">现在，先决条件已配置（本地 + Azure），可以完成部署。</p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto" _msttexthash="35812712" _msthash="386">远程（在 Azure 上）</h3><a id="user-content-remote-on-azure" class="anchor" aria-label="永久链接：远程（在 Azure 上）" href="#remote-on-azure" _mstaria-label="593411" _msthash="387"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto" _msttexthash="342063826" _msthash="388">GitHub Actions 上提供了预构建的容器映像，它将用于在 Azure 上部署解决方案：</p>
<ul dir="auto">
<li><font _mstmutation="1" _msttexthash="48601683" _msthash="389">来自分支的最新版本：</font><code>ghcr.io/clemlesne/call-center-ai:main</code></li>
<li><font _mstmutation="1" _msttexthash="55015883" _msthash="390">特定标签：（推荐）</font><code>ghcr.io/clemlesne/call-center-ai:0.1.0</code></li>
</ul>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto" _msttexthash="31741255" _msthash="391">1. 创建 light 配置文件</h4><a id="user-content-1-create-the-light-config-file" class="anchor" aria-label="永久链接： 1. 创建 light 配置文件" href="#1-create-the-light-config-file" _mstaria-label="1163266" _msthash="392"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font _mstmutation="1" _msttexthash="282213100" _msthash="393">本地配置文件名为 。安装脚本（包括 Makefile 和 Bicep）将使用它来配置 Azure 资源。</font><code>config.yaml</code></p>
<p dir="auto" _msttexthash="223741960" _msthash="394">使用以下内容填充文件（必须根据您的需要进行自定义）：</p>
<div class="highlight highlight-source-yaml notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-c"><span class="pl-c">#</span> config.yaml</span>
<span class="pl-ent">conversation</span>:
  <span class="pl-ent">initiate</span>:
    <span class="pl-c"><span class="pl-c">#</span> Phone number the bot will transfer the call to if customer asks for a human agent</span>
    <span class="pl-ent">agent_phone_number</span>: <span class="pl-s"><span class="pl-pds">"</span>+33612345678<span class="pl-pds">"</span></span>
    <span class="pl-ent">bot_company</span>: <span class="pl-s">Contoso</span>
    <span class="pl-ent">bot_name</span>: <span class="pl-s">Amélie</span>
    <span class="pl-ent">lang</span>: <span class="pl-s">{}</span>

<span class="pl-ent">communication_services</span>:
  <span class="pl-c"><span class="pl-c">#</span> Phone number purshased from Communication Services</span>
  <span class="pl-ent">phone_number</span>: <span class="pl-s"><span class="pl-pds">"</span>+33612345678<span class="pl-pds">"</span></span>

<span class="pl-ent">sms</span>: <span class="pl-s">{}</span>

<span class="pl-ent">prompts</span>:
  <span class="pl-ent">llm</span>: <span class="pl-s">{}</span>
  <span class="pl-ent">tts</span>: <span class="pl-s">{}</span></pre><div class="zeroclipboard-container">
   
  </div></div>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto" _msttexthash="22585745" _msthash="395">2. 连接到 Azure 环境</h4><a id="user-content-2-connect-to-your-azure-environment" class="anchor" aria-label="永久链接：2. 连接到 Azure 环境" href="#2-connect-to-your-azure-environment" _mstaria-label="1518361" _msthash="396"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>az login</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="az login" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto" _msttexthash="32866613" _msthash="397">3. 运行部署自动化</h4><a id="user-content-3-run-deployment-automation" class="anchor" aria-label="永久链接：3. 运行部署自动化" href="#3-run-deployment-automation" _mstaria-label="1142557" _msthash="398"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>make deploy name=my-rg-name</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="make deploy name=my-rg-name" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<ul dir="auto">
<li _msttexthash="21264347" _msthash="399">等待部署完成</li>
</ul>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto" _msttexthash="22063041" _msthash="400">4. <a href="https://learn.microsoft.com/en-us/azure/search/search-create-service-portal" rel="nofollow" _istranslated="1">创建 AI Search 资源</a></h4><a id="user-content-4-create-a-ai-search-resource" class="anchor" aria-label="永久链接：4. 创建 AI Search 资源" href="#4-create-a-ai-search-resource" _mstaria-label="1078103" _msthash="401"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ul dir="auto">
<li><font _mstmutation="1" _msttexthash="4040751" _msthash="402">名为</font><code>trainings</code></li>
<li><font _mstmutation="1" _msttexthash="4040751" _msthash="403">名为</font><code>default</code></li>
</ul>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto" _msttexthash="14302405" _msthash="404">5. 获取日志</h4><a id="user-content-5-get-the-logs" class="anchor" aria-label="永久链接：5. 获取日志" href="#5-get-the-logs" _mstaria-label="491062" _msthash="405"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>make logs name=my-rg-name</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="make logs name=my-rg-name" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto" _msttexthash="59072026" _msthash="406">本地（在您的计算机上）</h3><a id="user-content-local-on-your-machine" class="anchor" aria-label="永久链接：本地（在您的计算机上）" href="#local-on-your-machine" _mstaria-label="827879" _msthash="407"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto" _msttexthash="41164292" _msthash="408">1. 创建完整的配置文件</h4><a id="user-content-1-create-the-full-config-file" class="anchor" aria-label="永久链接：1. 创建完整的配置文件" href="#1-create-the-full-config-file" _mstaria-label="1107314" _msthash="409"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="markdown-alert markdown-alert-tip" dir="auto"><p class="markdown-alert-title" dir="auto"><svg class="octicon octicon-light-bulb mr-2" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="M8 1.5c-2.363 0-4 1.69-4 3.75 0 .984.424 1.625.984 2.304l.214.253c.223.264.47.556.673.848.284.411.537.896.621 1.49a.75.75 0 0 1-1.484.211c-.04-.282-.163-.547-.37-.847a8.456 8.456 0 0 0-.542-.68c-.084-.1-.173-.205-.268-.32C3.201 7.75 2.5 6.766 2.5 5.25 2.5 2.31 4.863 0 8 0s5.5 2.31 5.5 5.25c0 1.516-.701 2.5-1.328 3.259-.095.115-.184.22-.268.319-.207.245-.383.453-.541.681-.208.3-.33.565-.37.847a.751.751 0 0 1-1.485-.212c.084-.593.337-1.078.621-1.489.203-.292.45-.584.673-.848.075-.088.147-.173.213-.253.561-.679.985-1.32.985-2.304 0-2.06-1.637-3.75-4-3.75ZM5.75 12h4.5a.75.75 0 0 1 0 1.5h-4.5a.75.75 0 0 1 0-1.5ZM6 15.25a.75.75 0 0 1 .75-.75h2.5a.75.75 0 0 1 0 1.5h-2.5a.75.75 0 0 1-.75-.75Z"></path></svg><font _mstmutation="1" _msttexthash="5552768" _msthash="410">提示</font></p><p dir="auto"><font _mstmutation="1" _msttexthash="283188295" _msthash="411">若要使用服务主体向 Azure 进行身份验证，还可以在文件中添加以下内容：</font><code>.env</code></p>
<div class="highlight highlight-source-dotenv notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-v">AZURE_CLIENT_ID</span><span class="pl-k">=</span><span class="pl-s">xxx</span>
<span class="pl-v">AZURE_CLIENT_SECRET</span><span class="pl-k">=</span><span class="pl-s">xxx</span>
<span class="pl-v">AZURE_TENANT_ID</span><span class="pl-k">=</span><span class="pl-s">xxx</span></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="AZURE_CLIENT_ID=xxx
AZURE_CLIENT_SECRET=xxx
AZURE_TENANT_ID=xxx" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
</div>
<div class="markdown-alert markdown-alert-tip" dir="auto"><p class="markdown-alert-title" dir="auto"><svg class="octicon octicon-light-bulb mr-2" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="M8 1.5c-2.363 0-4 1.69-4 3.75 0 .984.424 1.625.984 2.304l.214.253c.223.264.47.556.673.848.284.411.537.896.621 1.49a.75.75 0 0 1-1.484.211c-.04-.282-.163-.547-.37-.847a8.456 8.456 0 0 0-.542-.68c-.084-.1-.173-.205-.268-.32C3.201 7.75 2.5 6.766 2.5 5.25 2.5 2.31 4.863 0 8 0s5.5 2.31 5.5 5.25c0 1.516-.701 2.5-1.328 3.259-.095.115-.184.22-.268.319-.207.245-.383.453-.541.681-.208.3-.33.565-.37.847a.751.751 0 0 1-1.485-.212c.084-.593.337-1.078.621-1.489.203-.292.45-.584.673-.848.075-.088.147-.173.213-.253.561-.679.985-1.32.985-2.304 0-2.06-1.637-3.75-4-3.75ZM5.75 12h4.5a.75.75 0 0 1 0 1.5h-4.5a.75.75 0 0 1 0-1.5ZM6 15.25a.75.75 0 0 1 .75-.75h2.5a.75.75 0 0 1 0 1.5h-2.5a.75.75 0 0 1-.75-.75Z"></path></svg><font _mstmutation="1" _msttexthash="5552768" _msthash="412">提示</font></p><p dir="auto"><font _mstmutation="1" _msttexthash="322200944" _msthash="413">如果应用程序已部署在 Azure 上，则可以运行以将配置从 Azure Function App 复制到本地计算机。</font><code>make name=my-rg-name sync-local-config</code></p>
</div>
<p dir="auto"><font _mstmutation="1" _msttexthash="40203553" _msthash="414">本地配置文件名为 ：</font><code>config.yaml</code></p>
<div class="highlight highlight-source-yaml notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-c"><span class="pl-c">#</span> config.yaml</span>
<span class="pl-ent">resources</span>:
  <span class="pl-ent">public_url</span>: <span class="pl-s">https://xxx.blob.core.windows.net/public</span>

<span class="pl-ent">conversation</span>:
  <span class="pl-ent">initiate</span>:
    <span class="pl-ent">agent_phone_number</span>: <span class="pl-s"><span class="pl-pds">"</span>+33612345678<span class="pl-pds">"</span></span>
    <span class="pl-ent">bot_company</span>: <span class="pl-s">Contoso</span>
    <span class="pl-ent">bot_name</span>: <span class="pl-s">Robert</span>

<span class="pl-ent">communication_services</span>:
  <span class="pl-ent">access_key</span>: <span class="pl-s">xxx</span>
  <span class="pl-ent">call_queue_name</span>: <span class="pl-s">call-33612345678</span>
  <span class="pl-ent">endpoint</span>: <span class="pl-s">https://xxx.france.communication.azure.com</span>
  <span class="pl-ent">phone_number</span>: <span class="pl-s"><span class="pl-pds">"</span>+33612345678<span class="pl-pds">"</span></span>
  <span class="pl-ent">post_queue_name</span>: <span class="pl-s">post-33612345678</span>
  <span class="pl-ent">recording_container_url</span>: <span class="pl-s">https://xxx.blob.core.windows.net/recordings</span>
  <span class="pl-ent">resource_id</span>: <span class="pl-s">xxx</span>
  <span class="pl-ent">sms_queue_name</span>: <span class="pl-s">sms-33612345678</span>

<span class="pl-ent">cognitive_service</span>:
  <span class="pl-c"><span class="pl-c">#</span> Must be of type "AI services multi-service account"</span>
  <span class="pl-ent">endpoint</span>: <span class="pl-s">https://xxx.cognitiveservices.azure.com</span>

<span class="pl-ent">llm</span>:
  <span class="pl-ent">fast</span>:
    <span class="pl-ent">mode</span>: <span class="pl-s">azure_openai</span>
    <span class="pl-ent">azure_openai</span>:
      <span class="pl-ent">context</span>: <span class="pl-c1">16385</span>
      <span class="pl-ent">deployment</span>: <span class="pl-s">gpt-4o-mini-2024-07-18</span>
      <span class="pl-ent">endpoint</span>: <span class="pl-s">https://xxx.openai.azure.com</span>
      <span class="pl-ent">model</span>: <span class="pl-s">gpt-4o-mini</span>
      <span class="pl-ent">streaming</span>: <span class="pl-c1">true</span>
  <span class="pl-ent">slow</span>:
    <span class="pl-ent">mode</span>: <span class="pl-s">azure_openai</span>
    <span class="pl-ent">azure_openai</span>:
      <span class="pl-ent">context</span>: <span class="pl-c1">128000</span>
      <span class="pl-ent">deployment</span>: <span class="pl-s">gpt-4o-2024-08-06</span>
      <span class="pl-ent">endpoint</span>: <span class="pl-s">https://xxx.openai.azure.com</span>
      <span class="pl-ent">model</span>: <span class="pl-s">gpt-4o</span>
      <span class="pl-ent">streaming</span>: <span class="pl-c1">true</span>

<span class="pl-ent">ai_search</span>:
  <span class="pl-ent">access_key</span>: <span class="pl-s">xxx</span>
  <span class="pl-ent">endpoint</span>: <span class="pl-s">https://xxx.search.windows.net</span>
  <span class="pl-ent">index</span>: <span class="pl-s">trainings</span>

<span class="pl-ent">ai_translation</span>:
  <span class="pl-ent">access_key</span>: <span class="pl-s">xxx</span>
  <span class="pl-ent">endpoint</span>: <span class="pl-s">https://xxx.cognitiveservices.azure.com</span></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="# config.yaml
resources:
  public_url: https://xxx.blob.core.windows.net/public

conversation:
  initiate:
    agent_phone_number: &quot;+33612345678&quot;
    bot_company: Contoso
    bot_name: Robert

communication_services:
  access_key: xxx
  call_queue_name: call-33612345678
  endpoint: https://xxx.france.communication.azure.com
  phone_number: &quot;+33612345678&quot;
  post_queue_name: post-33612345678
  recording_container_url: https://xxx.blob.core.windows.net/recordings
  resource_id: xxx
  sms_queue_name: sms-33612345678

cognitive_service:
  # Must be of type &quot;AI services multi-service account&quot;
  endpoint: https://xxx.cognitiveservices.azure.com

llm:
  fast:
    mode: azure_openai
    azure_openai:
      context: 16385
      deployment: gpt-4o-mini-2024-07-18
      endpoint: https://xxx.openai.azure.com
      model: gpt-4o-mini
      streaming: true
  slow:
    mode: azure_openai
    azure_openai:
      context: 128000
      deployment: gpt-4o-2024-08-06
      endpoint: https://xxx.openai.azure.com
      model: gpt-4o
      streaming: true

ai_search:
  access_key: xxx
  endpoint: https://xxx.search.windows.net
  index: trainings

ai_translation:
  access_key: xxx
  endpoint: https://xxx.cognitiveservices.azure.com" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto" _msttexthash="32866522" _msthash="415">2. 运行部署自动化</h4><a id="user-content-2-run-the-deployment-automation" class="anchor" aria-label="永久链接：2. 运行部署自动化" href="#2-run-the-deployment-automation" _mstaria-label="1323062" _msthash="416"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>make deploy-bicep deploy-post name=my-rg-name</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="make deploy-bicep deploy-post name=my-rg-name" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<ul dir="auto">
<li _msttexthash="292455566" _msthash="417">这将在没有 API 服务器的情况下部署 Azure 资源，从而允许您在本地测试机器人</li>
<li _msttexthash="21264347" _msthash="418">等待部署完成</li>
</ul>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto" _msttexthash="40221350" _msthash="419">3. 初始化本地函数配置</h4><a id="user-content-3-initialize-local-function-config" class="anchor" aria-label="永久链接：3. 初始化本地函数配置" href="#3-initialize-local-function-config" _mstaria-label="1488357" _msthash="420"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font _mstmutation="1" _msttexthash="67580500" _msthash="421">复制到 ，然后填写必填字段：</font><code>local.example.settings.json</code><code>local.settings.json</code></p>
<ul dir="auto">
<li><code>APPLICATIONINSIGHTS_CONNECTION_STRING</code><font _mstmutation="1" _msttexthash="98595575" _msthash="422">作为 Application Insights 资源的连接字符串</font></li>
<li><code>AzureWebJobsStorage</code><font _mstmutation="1" _msttexthash="67068287" _msthash="423">作为 Azure 存储帐户的连接字符串</font></li>
</ul>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto" _msttexthash="30920565" _msthash="424">4. 连接到 Azure Dev 隧道</h4><a id="user-content-4-connect-to-azure-dev-tunnels" class="anchor" aria-label="永久链接：4. 连接到 Azure Dev 隧道" href="#4-connect-to-azure-dev-tunnels" _mstaria-label="1177111" _msthash="425"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="markdown-alert markdown-alert-important" dir="auto"><p class="markdown-alert-title" dir="auto"><svg class="octicon octicon-report mr-2" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="M0 1.75C0 .784.784 0 1.75 0h12.5C15.216 0 16 .784 16 1.75v9.5A1.75 1.75 0 0 1 14.25 13H8.06l-2.573 2.573A1.458 1.458 0 0 1 3 14.543V13H1.75A1.75 1.75 0 0 1 0 11.25Zm1.75-.25a.25.25 0 0 0-.25.25v9.5c0 .138.112.25.25.25h2a.75.75 0 0 1 .75.75v2.19l2.72-2.72a.749.749 0 0 1 .53-.22h6.5a.25.25 0 0 0 .25-.25v-9.5a.25.25 0 0 0-.25-.25Zm7 2.25v2.5a.75.75 0 0 1-1.5 0v-2.5a.75.75 0 0 1 1.5 0ZM9 9a1 1 0 1 1-2 0 1 1 0 0 1 2 0Z"></path></svg><font _mstmutation="1" _msttexthash="7057479" _msthash="426">重要</font></p><p dir="auto" _msttexthash="198308058" _msthash="427">Tunnel 需要在单独的终端中运行，因为它需要一直运行</p>
</div>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-c"><span class="pl-c">#</span> Log in once</span>
devtunnel login

<span class="pl-c"><span class="pl-c">#</span> Start the tunnel</span>
make tunnel</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="# Log in once
devtunnel login

# Start the tunnel
make tunnel" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto" _msttexthash="36220015" _msthash="428">5. 使用代码快速迭代</h4><a id="user-content-5-iterate-quickly-with-the-code" class="anchor" aria-label="永久链接：5. 用代码快速迭代" href="#5-iterate-quickly-with-the-code" _mstaria-label="1244958" _msthash="429"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="markdown-alert markdown-alert-note" dir="auto"><p class="markdown-alert-title" dir="auto"><svg class="octicon octicon-info mr-2" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="M0 8a8 8 0 1 1 16 0A8 8 0 0 1 0 8Zm8-6.5a6.5 6.5 0 1 0 0 13 6.5 6.5 0 0 0 0-13ZM6.5 7.75A.75.75 0 0 1 7.25 7h1a.75.75 0 0 1 .75.75v2.75h.25a.75.75 0 0 1 0 1.5h-2a.75.75 0 0 1 0-1.5h.25v-2h-.25a.75.75 0 0 1-.75-.75ZM8 6a1 1 0 1 1 0-2 1 1 0 0 1 0 2Z"></path></svg><font _mstmutation="1" _msttexthash="5121168" _msthash="430">注意</font></p><p dir="auto"><font _mstmutation="1" _msttexthash="380279705" _msthash="431">要覆盖特定的配置值，您可以使用环境变量。例如，要覆盖该值，您可以使用变量：</font><code>llm.fast.endpoint</code><code>LLM__FAST__ENDPOINT</code></p>
<div class="highlight highlight-source-dotenv notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-v">LLM__FAST__ENDPOINT</span><span class="pl-k">=</span><span class="pl-s">https://xxx.openai.azure.com</span></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="LLM__FAST__ENDPOINT=https://xxx.openai.azure.com" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
</div>
<div class="markdown-alert markdown-alert-note" dir="auto"><p class="markdown-alert-title" dir="auto"><svg class="octicon octicon-info mr-2" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="M0 8a8 8 0 1 1 16 0A8 8 0 0 1 0 8Zm8-6.5a6.5 6.5 0 1 0 0 13 6.5 6.5 0 0 0 0-13ZM6.5 7.75A.75.75 0 0 1 7.25 7h1a.75.75 0 0 1 .75.75v2.75h.25a.75.75 0 0 1 0 1.5h-2a.75.75 0 0 1 0-1.5h.25v-2h-.25a.75.75 0 0 1-.75-.75ZM8 6a1 1 0 1 1 0-2 1 1 0 0 1 0 2Z"></path></svg><font _mstmutation="1" _msttexthash="5121168" _msthash="432">注意</font></p><p dir="auto"><font _mstmutation="1" _msttexthash="523468556" _msthash="433">此外，还可以使用脚本来测试应用程序，而无需打电话（= 没有通信服务）。使用以下命令运行脚本：</font><code>local.py</code></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>python3 -m tests.local</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="python3 -m tests.local" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
</div>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>make dev</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="make dev" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<ul dir="auto">
<li _msttexthash="164084960" _msthash="434">文件更改时会自动重新加载代码，无需重新启动服务器</li>
<li><font _mstmutation="1" _msttexthash="17018794" _msthash="435">API 服务器位于</font><code>http://localhost:8080</code></li>
</ul>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto" _msttexthash="14110226" _msthash="436">高级用法</h2><a id="user-content-advanced-usage" class="anchor" aria-label="永久链接：高级用法" href="#advanced-usage" _mstaria-label="545090" _msthash="437"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto" _msttexthash="23609248" _msthash="438">启用通话录音</h3><a id="user-content-enable-call-recording" class="anchor" aria-label="永久链接：启用通话录音" href="#enable-call-recording" _mstaria-label="812435" _msthash="439"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto" _msttexthash="155389442" _msthash="440">默认情况下，通话录音处于关闭状态。要启用它：</p>
<ol dir="auto">
<li><font _mstmutation="1" _msttexthash="402006462" _msthash="441">在 Azure 存储帐户中创建新容器（即 ），如果您在 Azure 上部署了解决方案，则它已经完成</font><code>recordings</code></li>
<li><font _mstmutation="1" _msttexthash="80244177" _msthash="442">将应用程序配置中的功能标志更新为</font><code>recording_enabled</code><code>true</code></li>
</ol>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto" _msttexthash="91547755" _msthash="443">使用 AI Search 添加我的自定义训练数据</h3><a id="user-content-add-my-custom-training-data-with-ai-search" class="anchor" aria-label="永久链接：使用 AI 搜索添加我的自定义训练数据" href="#add-my-custom-training-data-with-ai-search" _mstaria-label="1731769" _msthash="444"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto" _msttexthash="130498147" _msthash="445">训练数据存储在 AI Search 上，供机器人按需检索。</p>
<p dir="auto" _msttexthash="38010011" _msthash="446">所需的索引架构：</p>
<markdown-accessiblity-table data-catalyst=""><table>
<thead>
<tr>
<th><strong _msttexthash="11571014" _msthash="447">字段名称</strong></th>
<th><code>Type</code></th>
<th _msttexthash="5771792" _msthash="448">检索</th>
<th _msttexthash="5663684" _msthash="449">搜索</th>
<th _msttexthash="4597086" _msthash="450">尺寸</th>
<th _msttexthash="12038988" _msthash="451">矢量化器</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong _msttexthash="2873052" _msthash="452">答</strong></td>
<td><code>Edm.String</code></td>
<td _msttexthash="5535829" _msthash="453">是的</td>
<td _msttexthash="5535829" _msthash="454">是的</td>
<td></td>
<td></td>
</tr>
<tr>
<td><strong _msttexthash="6936761" _msthash="455">上下文</strong></td>
<td><code>Edm.String</code></td>
<td _msttexthash="5535829" _msthash="456">是的</td>
<td _msttexthash="5535829" _msthash="457">是的</td>
<td></td>
<td></td>
</tr>
<tr>
<td><strong _msttexthash="154869" _msthash="458">created_at</strong></td>
<td><code>Edm.String</code></td>
<td _msttexthash="5535829" _msthash="459">是的</td>
<td _msttexthash="1818271" _msthash="460">不</td>
<td></td>
<td></td>
</tr>
<tr>
<td><strong _msttexthash="396838" _msthash="461">document_synthesis</strong></td>
<td><code>Edm.String</code></td>
<td _msttexthash="5535829" _msthash="462">是的</td>
<td _msttexthash="5535829" _msthash="463">是的</td>
<td></td>
<td></td>
</tr>
<tr>
<td><strong _msttexthash="134810" _msthash="464">file_path</strong></td>
<td><code>Edm.String</code></td>
<td _msttexthash="5535829" _msthash="465">是的</td>
<td _msttexthash="1818271" _msthash="466">不</td>
<td></td>
<td></td>
</tr>
<tr>
<td><strong _msttexthash="9612486" _msthash="467">身份证</strong></td>
<td><code>Edm.String</code></td>
<td _msttexthash="5535829" _msthash="468">是的</td>
<td _msttexthash="1818271" _msthash="469">不</td>
<td></td>
<td></td>
</tr>
<tr>
<td><strong _msttexthash="7555418" _msthash="470">问题</strong></td>
<td><code>Edm.String</code></td>
<td _msttexthash="5535829" _msthash="471">是的</td>
<td _msttexthash="5535829" _msthash="472">是的</td>
<td></td>
<td></td>
</tr>
<tr>
<td><strong _msttexthash="5840419" _msthash="473">向量</strong></td>
<td><code>Collection(Edm.Single)</code></td>
<td _msttexthash="1818271" _msthash="474">不</td>
<td _msttexthash="5535829" _msthash="475">是的</td>
<td _msttexthash="22958" _msthash="476">1536</td>
<td><em _msttexthash="101673" _msthash="477">OpenAI ADA</em></td>
</tr>
</tbody>
</table></markdown-accessiblity-table>
<p dir="auto" _msttexthash="98665385" _msthash="478">用于填充索引的软件包含在 <a href="https://github.com/clemlesne/rag-index" _istranslated="1">Synthetic RAG Index 存储库中</a>。</p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto" _msttexthash="17518709" _msthash="479">自定义语言</h3><a id="user-content-customize-the-languages" class="anchor" aria-label="永久链接：自定义语言" href="#customize-the-languages" _mstaria-label="931931" _msthash="480"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto" _msttexthash="199744662" _msthash="481">该机器人可以在多种语言中使用。它可以理解用户选择的语言。</p>
<p dir="auto" _msttexthash="109623111" _msthash="482">请参阅 Text-to-Speech 服务<a href="https://learn.microsoft.com/en-us/azure/ai-services/speech-service/language-support?tabs=tts#supported-languages" rel="nofollow" _istranslated="1">支持的语言列表</a>。</p>
<div class="highlight highlight-source-yaml notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-c"><span class="pl-c">#</span> config.yaml</span>
<span class="pl-ent">conversation</span>:
  <span class="pl-ent">initiate</span>:
    <span class="pl-ent">lang</span>:
      <span class="pl-ent">default_short_code</span>: <span class="pl-s">fr-FR</span>
      <span class="pl-ent">availables</span>:
        - <span class="pl-ent">pronunciations_en</span>: <span class="pl-s">["French", "FR", "France"]</span>
          <span class="pl-ent">short_code</span>: <span class="pl-s">fr-FR</span>
          <span class="pl-ent">voice</span>: <span class="pl-s">fr-FR-DeniseNeural</span>
        - <span class="pl-ent">pronunciations_en</span>: <span class="pl-s">["Chinese", "ZH", "China"]</span>
          <span class="pl-ent">short_code</span>: <span class="pl-s">zh-CN</span>
          <span class="pl-ent">voice</span>: <span class="pl-s">zh-CN-XiaoqiuNeural</span></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="# config.yaml
conversation:
  initiate:
    lang:
      default_short_code: fr-FR
      availables:
        - pronunciations_en: [&quot;French&quot;, &quot;FR&quot;, &quot;France&quot;]
          short_code: fr-FR
          voice: fr-FR-DeniseNeural
        - pronunciations_en: [&quot;Chinese&quot;, &quot;ZH&quot;, &quot;China&quot;]
          short_code: zh-CN
          voice: zh-CN-XiaoqiuNeural" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font _mstmutation="1" _msttexthash="405887235" _msthash="483">如果生成并部署了 <a href="https://learn.microsoft.com/en-us/azure/ai-services/speech-service/custom-neural-voice" rel="nofollow" _mstmutation="1" _istranslated="1">Azure 语音自定义神经语音 （CNV），</a>请在语言配置上添加字段：</font><code>custom_voice_endpoint_id</code></p>
<div class="highlight highlight-source-yaml notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-c"><span class="pl-c">#</span> config.yaml</span>
<span class="pl-ent">conversation</span>:
  <span class="pl-ent">initiate</span>:
    <span class="pl-ent">lang</span>:
      <span class="pl-ent">default_short_code</span>: <span class="pl-s">fr-FR</span>
      <span class="pl-ent">availables</span>:
        - <span class="pl-ent">pronunciations_en</span>: <span class="pl-s">["French", "FR", "France"]</span>
          <span class="pl-ent">short_code</span>: <span class="pl-s">fr-FR</span>
          <span class="pl-ent">voice</span>: <span class="pl-s">xxx</span>
          <span class="pl-ent">custom_voice_endpoint_id</span>: <span class="pl-s">xxx</span></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="# config.yaml
conversation:
  initiate:
    lang:
      default_short_code: fr-FR
      availables:
        - pronunciations_en: [&quot;French&quot;, &quot;FR&quot;, &quot;France&quot;]
          short_code: fr-FR
          voice: xxx
          custom_voice_endpoint_id: xxx" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto" _msttexthash="23287628" _msthash="484">自定义审核级别</h3><a id="user-content-customize-the-moderation-levels" class="anchor" aria-label="永久链接：自定义审核级别" href="#customize-the-moderation-levels" _mstaria-label="1343290" _msthash="485"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto" _msttexthash="907055695" _msthash="486">为每个类别的内容安全定义了级别。分数越高，审核越严格，从 0 到 7。审核适用于所有机器人数据，包括网页和对话。在 Azure OpenAI 内容筛选器中配置它们。</p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto" _msttexthash="32858267" _msthash="487">自定义声明数据架构</h3><a id="user-content-customize-the-claim-data-schema" class="anchor" aria-label="永久链接：自定义声明数据架构" href="#customize-the-claim-data-schema" _mstaria-label="1250600" _msthash="488"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto" _msttexthash="302625908" _msthash="489">完全支持数据架构的自定义。您可以根据需要添加或删除字段，具体取决于要求。</p>
<p dir="auto" _msttexthash="106772133" _msthash="490">默认情况下，的 架构由以下部分组成：</p>
<ul dir="auto">
<li><code>caller_email</code> (<code>email</code>)</li>
<li><code>caller_name</code> (<code>text</code>)</li>
<li><code>caller_phone</code> (<code>phone_number</code>)</li>
</ul>
<p dir="auto" _msttexthash="153524267" _msthash="491">验证值以确保数据格式提交到您的架构。它们可以是：</p>
<ul dir="auto">
<li><code>datetime</code></li>
<li><code>email</code></li>
<li><code>phone_number</code> (<code>E164</code><font _mstmutation="1" _msttexthash="12597897" _msthash="492">格式）</font></li>
<li><code>text</code></li>
</ul>
<p dir="auto" _msttexthash="224825211" _msthash="493">最后，可以提供可选说明。描述必须简短且有意义，它将传递给 LLM。</p>
<p dir="auto" _msttexthash="92897246" _msthash="494">入站呼叫的默认架构在配置中定义：</p>
<div class="highlight highlight-source-yaml notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-c"><span class="pl-c">#</span> config.yaml</span>
<span class="pl-ent">conversation</span>:
  <span class="pl-ent">default_initiate</span>:
    <span class="pl-ent">claim</span>:
      - <span class="pl-ent">name</span>: <span class="pl-s">additional_notes</span>
        <span class="pl-ent">type</span>: <span class="pl-s">text</span>
        <span class="pl-c"><span class="pl-c">#</span> description: xxx</span>
      - <span class="pl-ent">name</span>: <span class="pl-s">device_info</span>
        <span class="pl-ent">type</span>: <span class="pl-s">text</span>
        <span class="pl-c"><span class="pl-c">#</span> description: xxx</span>
      - <span class="pl-ent">name</span>: <span class="pl-s">incident_datetime</span>
        <span class="pl-ent">type</span>: <span class="pl-s">datetime</span>
        <span class="pl-c"><span class="pl-c">#</span> description: xxx</span></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="# config.yaml
conversation:
  default_initiate:
    claim:
      - name: additional_notes
        type: text
        # description: xxx
      - name: device_info
        type: text
        # description: xxx
      - name: incident_datetime
        type: datetime
        # description: xxx" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font _mstmutation="1" _msttexthash="197921854" _msthash="495">通过在 API 调用中添加字段，可以为每个调用自定义声明架构。</font><code>claim</code><code>POST /call</code></p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto" _msttexthash="22943999" _msthash="496">自定义呼叫目标</h3><a id="user-content-customize-the-call-objective" class="anchor" aria-label="永久链接：自定义调用目标" href="#customize-the-call-objective" _mstaria-label="1147081" _msthash="497"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto" _msttexthash="530551008" _msthash="498">目标是机器人在通话期间将执行的操作的描述。它用于为 LLM 提供上下文。它应该简短、有意义，并且用英文书写。</p>
<p dir="auto" _msttexthash="109453448" _msthash="499">此解决方案是特权，而不是覆盖 LLM 提示符。</p>
<p dir="auto" _msttexthash="90702339" _msthash="500">入站呼叫的默认任务在配置中定义：</p>
<div class="highlight highlight-source-yaml notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-c"><span class="pl-c">#</span> config.yaml</span>
<span class="pl-ent">conversation</span>:
  <span class="pl-ent">initiate</span>:
    <span class="pl-ent">task</span>: <span class="pl-s">|</span>
<span class="pl-s">      Help the customer with their insurance claim. Assistant requires data from the customer to fill the claim. The latest claim data will be given. Assistant role is not over until all the relevant data is gathered.</span></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="# config.yaml
conversation:
  initiate:
    task: |
      Help the customer with their insurance claim. Assistant requires data from the customer to fill the claim. The latest claim data will be given. Assistant role is not over until all the relevant data is gathered." tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font _mstmutation="1" _msttexthash="154945817" _msthash="501">通过在 API 调用中添加字段，可以为每个调用自定义 Task。</font><code>task</code><code>POST /call</code></p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto" _msttexthash="15991040" _msthash="502">自定义对话</h3><a id="user-content-customize-the-conversation" class="anchor" aria-label="永久链接：自定义对话" href="#customize-the-conversation" _mstaria-label="1110304" _msthash="503"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto" _msttexthash="923990938" _msthash="504">对话选项表示为功能。它们可以通过应用程序配置进行配置，而无需重新部署或重新启动应用程序。更新功能后，需要延迟 60 秒才能使更改生效。</p>
<p dir="auto"><font _mstmutation="1" _msttexthash="4051880976" _msthash="505">|姓名 |描述 |类型 |默认 |
|-|-|-|
| |机器人应答的硬超时（以秒为单位）。| |180 元 |
| |机器人应答的软超时（以秒为单位）。| |30 元 |
| |回调的超时时间（以小时为单位）。| |72 元 |
| |电话静音的超时时间（以秒为单位）。| |1 |
| |是否开启通话录音。| |假 |
| |是否使用较慢的 LLM 进行聊天。| |真 |
| |语音识别的最大重试次数。| |2 |</font><code>answer_hard_timeout_sec</code><code>int</code><code>answer_soft_timeout_sec</code><code>int</code><code>callback_timeout_hour</code><code>int</code><code>phone_silence_timeout_sec</code><code>int</code><code>recording_enabled</code><code>bool</code><code>slow_llm_for_chat</code><code>bool</code><code>voice_recognition_retry_max</code><code>int</code></p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto" _msttexthash="33243561" _msthash="506">将 OpenAI 兼容模型用于 LLM</h3><a id="user-content-use-an-openai-compatible-model-for-the-llm" class="anchor" aria-label="永久链接：为 LLM 使用 OpenAI 兼容模型" href="#use-an-openai-compatible-model-for-the-llm" _mstaria-label="1696227" _msthash="507"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto" _msttexthash="310099244" _msthash="508">要使用与 OpenAI 补全 API 兼容的模型，您需要创建一个账户并获取以下信息：</p>
<ul dir="auto">
<li _msttexthash="8518575" _msthash="509">API 密钥</li>
<li _msttexthash="21630687" _msthash="510">上下文窗口大小</li>
<li _msttexthash="5896462" _msthash="511">端点 URL</li>
<li _msttexthash="10850450" _msthash="512">型号名称</li>
<li _msttexthash="19779344" _msthash="513">流式处理功能</li>
</ul>
<p dir="auto"><font _mstmutation="1" _msttexthash="71195150" _msthash="514">然后，在文件中添加以下内容：</font><code>config.yaml</code></p>
<div class="highlight highlight-source-yaml notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-c"><span class="pl-c">#</span> config.yaml</span>
<span class="pl-ent">llm</span>:
  <span class="pl-ent">fast</span>:
    <span class="pl-ent">mode</span>: <span class="pl-s">openai</span>
    <span class="pl-ent">openai</span>:
      <span class="pl-ent">context</span>: <span class="pl-c1">128000</span>
      <span class="pl-ent">endpoint</span>: <span class="pl-s">https://api.openai.com</span>
      <span class="pl-ent">model</span>: <span class="pl-s">gpt-4o-mini</span>
      <span class="pl-ent">streaming</span>: <span class="pl-c1">true</span>
  <span class="pl-ent">slow</span>:
    <span class="pl-ent">mode</span>: <span class="pl-s">openai</span>
    <span class="pl-ent">openai</span>:
      <span class="pl-ent">context</span>: <span class="pl-c1">128000</span>
      <span class="pl-ent">endpoint</span>: <span class="pl-s">https://api.openai.com</span>
      <span class="pl-ent">model</span>: <span class="pl-s">gpt-4o</span>
      <span class="pl-ent">streaming</span>: <span class="pl-c1">true</span></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="# config.yaml
llm:
  fast:
    mode: openai
    openai:
      context: 128000
      endpoint: https://api.openai.com
      model: gpt-4o-mini
      streaming: true
  slow:
    mode: openai
    openai:
      context: 128000
      endpoint: https://api.openai.com
      model: gpt-4o
      streaming: true" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto" _msttexthash="31075005" _msthash="515">使用 Twilio 进行短信</h3><a id="user-content-use-twilio-for-sms" class="anchor" aria-label="永久链接：使用 Twilio 进行短信" href="#use-twilio-for-sms" _mstaria-label="612534" _msthash="516"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto" _msttexthash="230039875" _msthash="517">要使用 Twilio 进行短信，您需要创建一个帐户并获取以下信息：</p>
<ul dir="auto">
<li _msttexthash="4835077" _msthash="518">帐户 SID</li>
<li _msttexthash="22159163" _msthash="519">身份验证令牌</li>
<li _msttexthash="12962820" _msthash="520">电话号码</li>
</ul>
<p dir="auto"><font _mstmutation="1" _msttexthash="71195150" _msthash="521">然后，在文件中添加以下内容：</font><code>config.yaml</code></p>
<div class="highlight highlight-source-yaml notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-c"><span class="pl-c">#</span> config.yaml</span>
<span class="pl-ent">sms</span>:
  <span class="pl-ent">mode</span>: <span class="pl-s">twilio</span>
  <span class="pl-ent">twilio</span>:
    <span class="pl-ent">account_sid</span>: <span class="pl-s">xxx</span>
    <span class="pl-ent">auth_token</span>: <span class="pl-s">xxx</span>
    <span class="pl-ent">phone_number</span>: <span class="pl-s"><span class="pl-pds">"</span>+33612345678<span class="pl-pds">"</span></span></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="# config.yaml
sms:
  mode: twilio
  twilio:
    account_sid: xxx
    auth_token: xxx
    phone_number: &quot;+33612345678&quot;" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto" _msttexthash="15569697" _msthash="522">自定义提示</h3><a id="user-content-customize-the-prompts" class="anchor" aria-label="永久链接：自定义提示" href="#customize-the-prompts" _mstaria-label="852098" _msthash="523"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font _mstmutation="1" _msttexthash="453702509" _msthash="524">请注意，提示示例包含占位符。这些占位符将替换为具有相应数据的机器人。例如，在内部替换为 bot 名称。</font><code>{xxx}</code><code>{bot_name}</code></p>
<p dir="auto" _msttexthash="235852097" _msthash="525">请务必用英文编写所有 TTS 提示。此语言用作对话翻译的枢轴语言。</p>
<div class="highlight highlight-source-yaml notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-c"><span class="pl-c">#</span> config.yaml</span>
<span class="pl-ent">prompts</span>:
  <span class="pl-ent">tts</span>:
    <span class="pl-ent">hello_tpl</span>: <span class="pl-s">|</span>
<span class="pl-s">      Hello, I'm {bot_name}, from {bot_company}! I'm an IT support specialist.</span>
<span class="pl-s"></span>
<span class="pl-s">      Here's how I work: when I'm working, you'll hear a little music; then, at the beep, it's your turn to speak. You can speak to me naturally, I'll understand.</span>
<span class="pl-s"></span>
<span class="pl-s">      Examples:</span>
<span class="pl-s">      - "I've got a problem with my computer, it won't turn on".</span>
<span class="pl-s">      - "The external screen is flashing, I don't know why".</span>
<span class="pl-s"></span>
<span class="pl-s">      What's your problem?</span>
<span class="pl-s"></span>  <span class="pl-ent">llm</span>:
    <span class="pl-ent">default_system_tpl</span>: <span class="pl-s">|</span>
<span class="pl-s">      Assistant is called {bot_name} and is in a call center for the company {bot_company} as an expert with 20 years of experience in IT service.</span>
<span class="pl-s"></span>
<span class="pl-s">      # Context</span>
<span class="pl-s">      Today is {date}. Customer is calling from {phone_number}. Call center number is {bot_phone_number}.</span>
<span class="pl-s"></span>    <span class="pl-ent">chat_system_tpl</span>: <span class="pl-s">|</span>
<span class="pl-s">      # Objective</span>
<span class="pl-s">      Provide internal IT support to employees. Assistant requires data from the employee to provide IT support. The assistant's role is not over until the issue is resolved or the request is fulfilled.</span>
<span class="pl-s"></span>
<span class="pl-s">      # Rules</span>
<span class="pl-s">      - Answers in {default_lang}, even if the customer speaks another language</span>
<span class="pl-s">      - Cannot talk about any topic other than IT support</span>
<span class="pl-s">      - Is polite, helpful, and professional</span>
<span class="pl-s">      - Rephrase the employee's questions as statements and answer them</span>
<span class="pl-s">      - Use additional context to enhance the conversation with useful details</span>
<span class="pl-s">      - When the employee says a word and then spells out letters, this means that the word is written in the way the employee spelled it (e.g. "I work in Paris PARIS", "My name is John JOHN", "My email is Clemence CLEMENCE at gmail GMAIL dot com COM")</span>
<span class="pl-s">      - You work for {bot_company}, not someone else</span>
<span class="pl-s"></span>
<span class="pl-s">      # Required employee data to be gathered by the assistant</span>
<span class="pl-s">      - Department</span>
<span class="pl-s">      - Description of the IT issue or request</span>
<span class="pl-s">      - Employee name</span>
<span class="pl-s">      - Location</span>
<span class="pl-s"></span>
<span class="pl-s">      # General process to follow</span>
<span class="pl-s">      1. Gather information to know the employee's identity (e.g. name, department)</span>
<span class="pl-s">      2. Gather details about the IT issue or request to understand the situation (e.g. description, location)</span>
<span class="pl-s">      3. Provide initial troubleshooting steps or solutions</span>
<span class="pl-s">      4. Gather additional information if needed (e.g. error messages, screenshots)</span>
<span class="pl-s">      5. Be proactive and create reminders for follow-up or further assistance</span>
<span class="pl-s"></span>
<span class="pl-s">      # Support status</span>
<span class="pl-s">      {claim}</span>
<span class="pl-s"></span>
<span class="pl-s">      # Reminders</span>
<span class="pl-s">      {reminders}</span></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="# config.yaml
prompts:
  tts:
    hello_tpl: |
      Hello, I'm {bot_name}, from {bot_company}! I'm an IT support specialist.

      Here's how I work: when I'm working, you'll hear a little music; then, at the beep, it's your turn to speak. You can speak to me naturally, I'll understand.

      Examples:
      - &quot;I've got a problem with my computer, it won't turn on&quot;.
      - &quot;The external screen is flashing, I don't know why&quot;.

      What's your problem?
  llm:
    default_system_tpl: |
      Assistant is called {bot_name} and is in a call center for the company {bot_company} as an expert with 20 years of experience in IT service.

      # Context
      Today is {date}. Customer is calling from {phone_number}. Call center number is {bot_phone_number}.
    chat_system_tpl: |
      # Objective
      Provide internal IT support to employees. Assistant requires data from the employee to provide IT support. The assistant's role is not over until the issue is resolved or the request is fulfilled.

      # Rules
      - Answers in {default_lang}, even if the customer speaks another language
      - Cannot talk about any topic other than IT support
      - Is polite, helpful, and professional
      - Rephrase the employee's questions as statements and answer them
      - Use additional context to enhance the conversation with useful details
      - When the employee says a word and then spells out letters, this means that the word is written in the way the employee spelled it (e.g. &quot;I work in Paris PARIS&quot;, &quot;My name is John JOHN&quot;, &quot;My email is Clemence CLEMENCE at gmail GMAIL dot com COM&quot;)
      - You work for {bot_company}, not someone else

      # Required employee data to be gathered by the assistant
      - Department
      - Description of the IT issue or request
      - Employee name
      - Location

      # General process to follow
      1. Gather information to know the employee's identity (e.g. name, department)
      2. Gather details about the IT issue or request to understand the situation (e.g. description, location)
      3. Provide initial troubleshooting steps or solutions
      4. Gather additional information if needed (e.g. error messages, screenshots)
      5. Be proactive and create reminders for follow-up or further assistance

      # Support status
      {claim}

      # Reminders
      {reminders}" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto" _msttexthash="18964127" _msthash="526">优化响应延迟</h3><a id="user-content-optimize-response-delay" class="anchor" aria-label="永久链接：优化响应延迟" href="#optimize-response-delay" _mstaria-label="939809" _msthash="527"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto" _msttexthash="46499375" _msthash="528">延迟主要来自两件事：</p>
<ul dir="auto">
<li _msttexthash="1179867221" _msthash="529">事实上，Azure 通信服务在转发音频的方式上是连续的（从技术上讲，它只处理文本，而不是音频，并且一旦转换了整个音频，就会等待指定的空白时间）</li>
<li _msttexthash="2080660322" _msthash="530">LLM，更具体地说是 API 调用和推断的第一个句子之间的延迟，可能会很长（因为句子一旦可用，就会一个接一个地发送），如果它产生幻觉并返回空答案，则甚至更长（这种情况经常发生，并且 applicatoipn 会重试调用）</li>
</ul>
<p dir="auto"><font _mstmutation="1" _msttexthash="1416931230" _msthash="531">从现在开始，您唯一能做的就是 LLM 部分。这可以通过 Azure 上的 PTU 或使用不太智能的模型来实现，例如（在最新版本上默认选择）。使用 Azure OpenAI 上的 PTU，在某些情况下可以将延迟除以 2。</font><code>gpt-4o-mini</code></p>
<p dir="auto" _msttexthash="791606647" _msthash="532">该应用程序本机连接到 Azure Application Insights，因此您可以监控响应时间并查看时间花费在哪里。这是识别瓶颈的良好开端。</p>
<p dir="auto" _msttexthash="198413020" _msthash="533">如果您有任何优化响应延迟的想法，请随时提出问题或提出 PR。</p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto" _msttexthash="29954067" _msthash="534">Q&amp;A （问答）</h2><a id="user-content-qa" class="anchor" aria-label="永久链接：Q&amp;A" href="#qa" _mstaria-label="292682" _msthash="535"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto" _msttexthash="43194528" _msthash="536">为什么不使用 LLM 框架？</h3><a id="user-content-why-no-llm-framework-is-used" class="anchor" aria-label="永久链接：为什么不使用 LLM 框架？" href="#why-no-llm-framework-is-used" _mstaria-label="1057654" _msthash="537"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto" _msttexthash="1312311000" _msthash="538">在开发时，没有 LLM 框架可用于处理所有这些功能：具有多工具的流功能、可用性问题的备份模型、触发工具中的回调机制。因此，直接使用 OpenAI SDK，并实施了一些算法来处理可靠性。</p>
</article></div>
