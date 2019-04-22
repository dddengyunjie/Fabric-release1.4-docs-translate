 Blockchain network
 区块链网络
  This topic will describe, at a conceptual level, how Hyperledger Fabric allows organizations to collaborate in the formation of blockchain 
networks. If you’re an architect, administrator or developer, you can use this topic to get a solid understanding of the major structure 
and process components in a Hyperledger Fabric blockchain network. This topic will use a manageable worked example that introduces all of 
the major components in a blockchain network. After understanding this example you can read more detailed information about these 
components elsewhere in the documentation, or try building a sample network.                                                        
  这个专题将会在一个概念的层次描述超级账本fabric区块链网络在形成过程中如何允许组织之间的协作。如果你是一个架构师，管理员或开发人员，你能通过这个专题会对
fabric区块链网络的主架构和各个组件有一个更深入的理解。这个专题将会使用一个可管理的工作示例来介绍区块链网络中的主要组件。理解完这个例子你能在这个文档的其
它地方阅读更多关于这些组件的详细信息，或者试着创建一个示例网络。
  After reading this topic and understanding the concept of policies, you will have a solid understanding of the decisions that 
organizations need to make to establish the policies that control a deployed Hyperledger Fabric network. You’ll also understand how 
organizations manage network evolution using declarative policies – a key feature of Hyperledger Fabric. In a nutshell, you’ll understand 
the major technical components of Hyperledger Fabric and the decisions organizations need to make about them.
  读完这个专题并理解策略的概念后，你将会对组织需要制定一个策略用于管控一个部署好的fabric网络有一个更深入的理解。你同时也会更加理解一个组织如何使用声明
性的策略来管理网络演变（fabric的一个关键的特性）。简而言之，你将会理解fabric网络的主要技术组件和组织需要对它们所制定的决策。

What is a blockchain network?
什么是区块链网络
  A blockchain network is a technical infrastructure that provides ledger and smart contract (chaincode) services to applications. 
Primarily, smart contracts are used to generate transactions which are subsequently distributed to every peer node in the network where
they are immutably recorded on their copy of the ledger. The users of applications might be end users using client applications or 
blockchain network administrators.
  区块链网络是一个向应用程序提供账本和智能合约（链码）的技术性的基础设施。首先，智能合约用于生成交易，这些交易随后都会分发到网络上的每个节点并生成不可
篡改的记录。应用的使用者们可能是应用的终端用户或者是区块链网络管理员。
  In most cases, multiple organizations come together as a consortium to form the network and their permissions are determined by a set 
of policies that are agreed by the consortium when the network is originally configured. Moreover, network policies can change over time
subject to the agreement of the organizations in the consortium, as we’ll discover when we discuss the concept of modification policy.
  在大多数情况下，多个组织组合成一个联盟来形成一个网络并且他们的权限由一组策略决定，这些策略是由联盟在网络最初生成时的配置决定。接下来当我们讨论修改策略
的概念时，我们将会发现，此外网络策略也可以通过联盟中的各个组织的统一同意下进行修改。
