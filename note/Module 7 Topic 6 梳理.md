# Module 7 Topic 6

Hot topics in Service Computing - Cloud

Topic 6: Problems with cloud computing - Security Issues in Cloud Computing

[TOC]

## 1 Cloud Computing: A Massive Concentration of Resources

云计算：资源的大规模集中

- Also a massive concentration of risk
  - expected loss from a single breach can be significantly larger
  - concentration of “users” represents a concentration of threats
- “Ultimately, you can outsource responsibility but you can’t outsource accountability.”

---

responsibility 可以翻译为职责，指的是谁要做这个活；而 accountability 翻译为可追责性，指的是，这个活干得好不好（尤其是没干好的时候），谁负总体责任，这个负总体责任的人不一定是具体干活的人。

找了个例子，供参考：

妈妈叫你和弟弟及妹妹三人一起把房间卫生打扫一下，这时你们三人都是 responsible。

如果妈妈只交待让你们仨搞下卫生，谁都会想「我先去忙会儿别的，反正还有其他两个人」，到头来谁都不会去做，哪怕做了，也是马马虎虎做，因为就算做砸了，妈妈也不会责怪我一个人嘛。

但是如果妈妈说「你们兄妹仨一起搞下卫生，小明你作为哥哥，总负责一下，如果回来我看见房间还是脏的，那就要打你屁股了」，这时三个人都是 responsible，然而只有你是 accountable。这时你就会好好管理好弟弟妹妹的工作，并且还会仔细检查工作是不是到位了。

所以这里的意思是，你可以把活交给外包的服务商干，但是你不能把负责总体责任的任务外包。

## 2 Threats & Vulnerabilities

**Vulnerability** is any weakness in information system, system security procedures, internal controls or implementation that could be exploited or triggered by a threat resources.

- Insufficient due diligence
- Misconfigured cloud services
- Insecure interface 
- Obsolete cryptography 
- Insecure VM migration 
- Internet protocol 
- Vendor lock-in 
- …

**Threat** is harm or unauthorized access that might occur due to vulnerability and destroy organization assets, organization operations or system information.

## 3 Cloud Computing: who should use it?

## 4 Problems Associated with Cloud Computing

- Most security problems stem from:
  - Loss of control
  - Lack of trust (mechanisms)
  - Multi-tenancy
- These problems exist mainly in 3rd party management models
  - Self-managed clouds still have security issues, but not related to above

## 5 Conclusion

- Cloud computing is sometimes viewed as a version of the classic mainframe client-server model
  - However, resources are ubiquitous, scalable, highly virtualized
  - Contains all the traditional threats, as well as new ones
- In developing solutions to cloud computing security issues it may be helpful to identify the problems and approaches in terms of
  - Loss of control
  - Lack of trust
  - Multi-tenancy problems