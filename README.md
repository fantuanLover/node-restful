# node-restful
工作流程是这样的<br />
router(express拦截请求) => helper(Joi做信息验证) => passport中间件(passport做jwt授权验证) => controller(做业务处理) => model(mongoose)<br />
待添加事项<br />
1.TDD开发(特别想做这块儿，在北京找工作不知道能不能有充足的时间做完)<br />
2.做service层，把一些业务从controller抽离(主要是model层相关的一些业务)<br />
PS.为什么要分离service层,我的看法是方便测试.如果把功能函数放在controller,要mock的时候需要模拟http请求过程,如果把功能直接写成纯函数放在service层,只需要一般的unittest就可以完成测试.

