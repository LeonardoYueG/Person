## 秋招

经过5个月的秋招之旅，现在拿到手的就一个手机厂的offer，而且这个offer来的也是因为自己运气好的原因

反思自己的整个秋招之旅最大的问题还是自己性格问题，江山易改本性难移，后面8个月要做重要事情很多的事情

1.六级最后一次机会过了，不过很多单位都卡六级（银行、研究所、国企）

2.春招，可能是这辈子最容易改变自己人生的一件事了，不管是读博还是工作，改变自己是最重要的，选一个方向，改变自己的陋习

3.毕业，感觉这两年多过的浑浑噩噩，没有一开始那股冲劲，因为种种原因（没有找工作的经验、错误信息的误导（网上和师兄的反馈，嗯应该听小师兄的）and so on）导致自己没有一个积极找工作的态度和紧迫感，导致这次春招的失利。

## 给自己定一个目标

春招找一份：大厂（阿里、腾讯、字节、美团、快手、拼多多、京东和其他的）、有前景（到底从事什么方向Java、android、算法、前端、后端、and so on一定要慎重思考并快速做出决定，毕竟时间不等人还有毕业论文和春招，时间就是声明，so quickly）,不要让自己成为一个废物，第一份工作很重要，你要成为一个leader，你也要先成为一个技术达人，OK？，so现在首先要做的就是确定方向

## 技术方向

- Android：现在最好转就是Android因为Java开发自己也不会，都是从新学，所以目前android目前是一个好转的方向。Android：新要求：参与各类跨平台框架/动态化技术的研发，包括但不限于浏览器内核、Flutter、ReactNative、Hybrid容器等
- Java后端：再其次是Java后端（卷中卷），但是Java后端现在很卷，所以春招的时候Java后端的情况会怎样，现在还没有一个确定情况，整个要考虑清楚。
- CV算法：算法反而没有Java卷，但是CV在算法中很卷，推荐算法和NLP没有那么卷，为什么选择了一个这样的方向，主要是因为自己前期没有做好调查（具体转方向需要做好调查，而且需要考虑如何做调查）
- C++：C++不太了解，是否能够半年能有一定的掌握和竞争力有待考究，而且C++春招情况会怎么样，也不太确定，但是C++会出现前面的白学了，和之前算法一样，所以你一定要考虑清楚。
- 前端：前端完全没有接触过，但是前端需要学习的东西不太多，能快速上手，但是问题就是快速上手的东西门槛相对较低。
- ~~深度学习的移动端~~：整个是被划到算法里面了，还是可以算法和移动端结合，需要查一下资料才能明白（好像没有这个方向）

## 现在急需解决的问题

### 确定方向

| **方向** |              **发展前景**              |              **竞争情况**              |    **学习成本**    |
| :------: | :------------------------------------: | :------------------------------------: | :----------------: |
| Android  |           一般，普通而已开发           | 不激烈（但是明年春招情况如何不太了解） |      相对较低      |
| Java后端 |         一般，比Android好一点          |                竞争激烈                | 需要学的东西太多了 |
|  CV算法  |            发展前景相对较好            |                竞争激烈                |   需要学东西较多   |
|   C++    |              发展前景不错              |              竞争相对较小              |   需要全部从新学   |
|   前端   |            一般，就普通开发            |              竞争相对较小              |  但是需要从0开始   |
|   读博   | 前景不错，关键问题（方向、老师、学校） |              竞争相对较小              |     高，非常高     |

### 需要改掉的陋习

- **做事拖沓**：不管以后干什么这个问题一定要解决，做事情一定快并且有效率，不要懒床（有一个确定的时间表，不要睡前起床玩手机）、不要玩手机（手机以后能不带尽量不要带，没人找你OK？）
- **解决问题的能力不强**：coding能力一定要提上去，不要老是想着粘贴复制看看其他人的解决方案，还有就是leetcode和牛客一定要刷
- **不要想那些乱七八糟的**：你未来5年的任务是做到一个领域的技术leader，这样你后面的人生才有一定的保障

```java
public class Singleton {

    //volatile保证，当uniqueInstance变量被初始化成Singleton实例时，多个线程可以正确处理uniqueInstance变量
    private volatile static Singleton uniqueInstance;
    private Singleton() {
    }
    public static Singleton getInstance() {
       //检查实例，如果不存在，就进入同步代码块
        if (uniqueInstance == null) {
            //只有第一次才彻底执行这里的代码
            synchronized(Singleton.class) {
               //进入同步代码块后，再检查一次，如果仍是null，才创建实例
                if (uniqueInstance == null) {
                    uniqueInstance = new Singleton();
                }
            }
        }
        return uniqueInstance;
    }
}
```

