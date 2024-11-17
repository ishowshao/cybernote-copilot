# cybernote-copilot

## API dev

* `/api/note/embed?model={string}&id={uuid}&title={string}&content={string}`
    * note拆解和向量化后存入embedding database，content不需要存，只需要存id
* `/api/note/search?query={string}&limit={int}`
    * query向量化后，去embedding database检索
* `/api/structure?input=`
    * 对input进行结构化整理
* `/api/summarize?input=`
    * 对input进行概括
* `/api/completion?prompt=&input=`
    * 对input进行补全，可以添加prompt，prompt可以为空