# NoFakeChain (nfChain), the next generation of Blockchain for e-commerce.

A new protocol that tackles today’s biggest social and economic problems and which provides:
1.	Anti-counterfeiting support: 20% of on-line purchases are fake, 10% of global trade is in bogus goods and services. 
1.	Product tracing: Gives back control to the stake holders by linking the actual real world object with Blockchain objects
1.	Supply chain transparency: Removes information silos and builds open and readily accessible platforms
1.	Support for small and medium enterprise (SME) finance: Produces a diversified and healthy Blockchain ecosystem
1.	Support for second hand goods market: To create a sustainable world
 
Technical standards:
1.	Mixed Chain Technology and Transaction Tunnelling
1.	Proof of Relevance algorithms
1.	ASIC resistant and mobile friendly mining
1.	Developer friendly and safe, smart contract programming language
1.	High performing VM

# NoFakeChain (nfChain), 新一代电商区块链

该协议解决当前人类最大的社会和经济问题：

1.	防伪: 20% 的在线商品为假货, 全球贸易的10%为假货 
1.	溯源: 通过链接产品和区块链对象，让贸易相关方都参与进来
1.	供应链管理: 消灭信息孤岛，建立世界大同的平等开放的平台
1.	中小企业融资:建立一个多样性的健康区块链生态
1.	二手交易市场: 为了一个可持续的未来

技术标准
1.	混合链以及交易隧道
2.  相关性证明共识算法(Proof of Relevance algorithms)
3.	支持移动设备的挖矿算法(ASIC resistant and mobile friendly mining)
4.	友好且安全的智能合约语言
5.	高效虚拟机


# NoFakeChain (nfChain), 次世代の電子商用プラットフォーム用ブロックチェーン

今の最大の社会的、経済的問題を解決する新しいプロトコル：
1.	偽造防止：オンライン購入の20％が偽物であり、世界の取引の10％が偽造されています。
1.	製品トレース：世界の実際のオブジェクトをブロックチェーンオブジェクトにリンクすることによって、ステークホルダーにコントロールを返す
1.	サプライチェーン：情報サイロを取り除き、オープンで同等のプラットフォームを構築する
1.	中小企業金融：多様で健全なブロックチェーンの生態系を創る
1.	中古市場：持続可能な世界を創造する

高い基準
1.	混合チェーン技術とトランザクショントンネル
1.	関連性证明共存算法(Proof of Relevance algorithms)
1.	ASIC耐性とモバイルフレンドリーなマイニング
1.	開発者フレンドリーで安全なスマート契約プログラミング言語
1.	高性能仮想マシン

# NoFakeChain (nfChain), 노 페이크 투데이(No Fake Today),　
더 이상 가짜짝퉁은 존재하지 않는다.
차세대 전자 상거래 플랫폼, Blockchain
 2016년OECD통계에 의하면 전세계 가짜짝통시장은 4610억달러(522조5435억원)에 달하고 있습니다.

NFT코인은 현대의 가장 큰 사회적, 경제적 고민거리를 해결할 수 있는 획기적인 프로토콜 :
1.	위조 방지 : 온라인상 구매명품의 20 %가 가짜이며 전세계 명품거래의 10 %가 위조제품입니다.
1.	상품 추적 : 전세계의 상품개체를 Blockchain으로 연결하여 상품의 오리지날증명이 가능하여 스테이크홀더가 각자 시스템컨트롤이 가능
1.	공급 체인 : 불안전하고 고립된 정보 체계를 제거하고 개방적이고 평등한 플랫폼 구축
1.	중소기업 금융 : 다양하고 건강한 블록 체인 에코시스템을 구축
1.	중고 시장 : 지속 가능한 세계를 창조하기 위해 마련

엄격한 기준

1.	각기 다른 블론체인 기술의 혼합 및 트랜잭션 터널
1.	관련성 일치 알고리즘 증명
1.	ASIC 내성 및 모바일 친화적인 채광
1.	개발자친화적이고 안전한 스마트 계약 프로그래밍 언어
1.	고성능 VM


<a href="https://nofake.today/architecture.jpg" target="_blank" rel="noopener"><img title="architecture" src="https://nofake.today/architecture.jpg" alt="architecture" /></a>

nfChain is an Ethereum-based distributed ledger protocol with transaction/contract privacy and new consensus mechanisms.

nfChain is a fork of [go-ethereum](https://github.com/ethereum/go-ethereum) and is updated in line with go-ethereum releases.

Key enhancements over go-ethereum:

  * __Privacy__ - nfChain supports private transactions via a Transaction Tunnel, a peer-to-peer encrypted message tunnel for directed transfer of private data to network counterparties
  * __Alternative Consensus Mechanisms__ - Instead of using POW/POS as a consensus algo, nfChain offers multiple consensus options that are appropriate for consortium chains:
    * __Prove of Relevance Consensus__ - a consensus model for highly performance, scalability, transaction finality, and on-demand block creation
    * __Raft-based Consensus__ - a consensus model for faster blocktimes, transaction finality, and on-demand block creation
    * __Applied BFT__ - a PBFT-inspired consensus algorithm.
  * __Peer Permissioning__ - node/peer permissioning using smart contracts, ensuring only known parties can join the network
  * __Higher Performance__ - nfChain offers significantly higher performance than public geth

Note: The nfChain consensus algorithm is not yet supported by this release.

## Architecture


The above diagram is a high-level overview of the privacy architecture used by nfChain. For more in-depth discussion of the components, refer to the [wiki](https://github.com/) pages.

## Quickstart

The quickest way to get started with nfChain is using [VirtualBox](https://www.virtualbox.org/wiki/Downloads) and [Vagrant](https://www.vagrantup.com/downloads.html):

```sh
git clone https://github.com/nofaketoday/nfChain
cd nfChain-examples
vagrant up
# (should take 5 or so minutes)
vagrant ssh
```

Now that you have a fully-functional nfChain environment, let's run a cluster with 17 nodes. This will spin up several nodes with a mix of voters, leader, and unprivileged nodes.

```sh
# (from within vagrant env, use `vagrant ssh` to enter)
$ cd nfChain-examples/17nodes

$ ./nf-start.sh
[*] Cleaning up temporary data directories
[*] Configuring node 1 (permissioned) as voter
INFO [2017-05-30|22:08:59] Allocated cache and file handles         database=...
INFO [2017-05-30|22:08:59] Writing custom genesis block 
INFO [2017-05-30|22:08:59] Successfully wrote genesis state         database=chaindata                                                    hash=c23b4e…8b1b71
INFO [2017-05-30|22:08:59] Allocated cache and file handles         database=...
INFO [2017-05-30|22:08:59] Writing custom genesis block 
INFO [2017-05-30|22:08:59] Successfully wrote genesis state         database=lightchaindata                                                    hash=c23b4e…8b1b71

[*] Configuring node 2 (permissioned) as leader for blocking creator
...

[*] Configuring node 3
WARN [2017-05-30|22:08:59] Not permissioned hence reduced blocking reward 

[*] Configuring node 4
WARN [2017-05-30|22:08:59] Coinbase not found
WARN [2017-05-30|22:08:59] Not permissioned hence reduced blocking reward 

...

[*] Configuring node 5 (permissioned) as voter
[*] Configuring node 6 (permissioned) as voter
[*] Configuring node 7 (permissioned) as voter
[*] Configuring node 8 (permissioned) as voter
[*] Configuring node 9 (permissioned) as voter
[*] Configuring node 10 (permissioned) as voter
[*] Configuring node 11 (permissioned) as voter
[*] Configuring node 12 (permissioned) as voter
[*] Configuring node 13 (permissioned) as voter
...
[*] Configuring node 17 (permissioned) as voter


[*] Starting Constellation nodes
[*] Starting node 1 (permissioned)
[*] Starting node 2 (permissioned)
[*] Starting node 3 (not permissioned)
[*] Starting node 4 (not permissioned)
[*] Starting node 5 (permissioned)
[*] Starting node 6 (permissioned)
...
[*] Starting node 17 (permissioned)
[*] Waiting for nodes to start
...
All pre-defined nodes are up. 
Log dir: 'dataDir/logs' for logs, 
'geth attach dataDir/nodeX/geth.ipc' to attach to the node X
...
[*] Processing transaction.
INFO [2017-05-30|22:08:59]TransactionHash: 0xfd8198bfb875398ff23d58d0d4fd5a1e7789dadb18b0a378fb98c2c38ff3d42e waiting to be mined...
INFO [2017-05-30|22:08:59] mined

```

Now we can see 17-node nfChain cluster is up and running. And there is product sent from `node 1` "for" `node 5` for processing.

Let's connect to one of the nodes and inspect:

```sh
$ geth attach ipc:dataDir/node11/geth.ipc
Welcome to the Geth JavaScript console!

instance: Geth/v1.6.0-stable-facc47c/linux/go1.7.0
coinbase: 0x0ae08537e544d1466a545f5986977cc5b27e46e9
at block: 1 (Tue, 30 May 2017 22:09:03)
 datadir: dataDir/node1
 modules: admin:1.0 debug:1.0 eth:1.0 net:1.0 personal:1.0 nfChain:1.0 rpc:1.0 txpool:1.0 web3:1.0

> nfChain.nodeInfo
{
  blockMakerAccount: "0x0ae08537e544d1466a545f5986977cc5b27e46e9",
  blockmakestrategy: {
    maxblocktime: 10,
    minblocktime: 3,
    status: "active",
    type: "deadline"
  },
  canCreateBlocks: true,
  canVote: true,
  voteAccount: "0x5d646f0d090d510b34c76688d0665473fd8590f7"
}

# get private txn created earlier:
> eth.getTransaction('0xfd8198bfb875398ff23d58d0d4fd5a1e7789dadb18b0a378fb98c2c38ff3d42e')
{
  blockHash: "0xd311518d7a12afe64627ca1d2f77e924e4fad6ee63972add9a6a40c783a9b0ca",
  blockNumber: 1,
  from: "0xb33d92f29446d8fb696fa85e02530199badda88d",
  gas: 4700000,
  gasPrice: 0,
  hash: "0xfd8198bfb875398ff23d58d0d4fd5a1e7789dadb18b0a378fb98c2c38ff3d42e",
  input: "0x664ede7b6cbd5f5fd3c4c0608ce2e8d03a65f02e024724b1cd7c7db7f44e07288197cb0637e3f49305eb17cfde7a4bb9eb51896af2761db9e6df53180e9f3560",
  nonce: 0,
  r: "0x449327f6ce32fa3bf55a9f871ee56ad2c229e2f9c778b686eec437308fc54ac1",
  s: "0x352b35e6b4058f53d8c0bc7c58afb3356f7677377a334655400377fef0090f7e",
  to: null,
  transactionIndex: 0,
  v: "0x26",
  value: 0
}

```


## Anti-counterfeiting 
The details can be found here [Features](https://nofake.today).

## Product tracing 
The details can be found here [Features](https://nofake.today).

## Supply chain transparency 
The details can be found here [Features](https://nofake.today).

## Product tracing 
The details can be found here [Features](https://nofake.today).

## Proof of relevance  
The details can be found here [Features](https://nofake.today).

## Further Reading
Further documentation can be found in the [Readings](https://nofake.today) 


## Contributing
Any contribution to nfChain is appreciated!
nfChain is built on open source and we invite you to contribute enhancements. Upon review you will be required to complete a Contributor License Agreement (CLA) before we are able to merge. If you have any questions about the contribution process, please feel free to send an email to us.

## License
The go-ethereum library (i.e. all code outside of the `cmd` directory) is licensed under the
[GNU Lesser General Public License v3.0](https://www.gnu.org/licenses/lgpl-3.0.en.html), also
included in our repository in the `COPYING.LESSER` file.

The go-ethereum binaries (i.e. all code inside of the `cmd` directory) is licensed under the
[GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.en.html), also included
in our repository in the `COPYING` file.
