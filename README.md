# Repolex Knowledge Graph of tokio-rs/tokio

RDF knowledge graph data for [tokio-rs/tokio](https://github.com/tokio-rs/tokio), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [lexq](https://github.com/repolex-ai/lexq) query tool using [uv](https://docs.astral.sh/uv/getting-started/installation/).

If you have uv installed, just copy/paste this into your terminal:

```bash
uv tool install git+https://github.com/repolex-ai/lexq
```

This installs lexq onto your system, in your user context. Verify the install:

```bash
lexq --help
```

**lexq is designed to be used primarily by LLMs in a terminal.** Start up your favorite LLM and ask it to use the lexq tool. It's that easy!

To load this repo's data:

```bash
lexq download tokio-rs/tokio
```

This will automatically download essential data files from the last parsed commit. Consult `lexq --moreinfo` for other options, including downloading multiple commits, blobs, etc.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   ├── 6847ed76ce77eb9fba10bf954c23058c6949d463.nq.gz
│   │   └── b47ad242686a7f1850c724f691d8cd948f08f47f
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   ├── 6847ed76ce77eb9fba10bf954c23058c6949d463.nq.gz
│   │   └── b47ad242686a7f1850c724f691d8cd948f08f47f.nq.gz
│   └── repolex
│       ├── 6847ed76ce77eb9fba10bf954c23058c6949d463.nq.gz
│       └── b47ad242686a7f1850c724f691d8cd948f08f47f
│           └── chunk-001.nq.gz
└── blob
    ├── 0227c14e841be4b185fcce2a00dda522c2e83848.nq.gz
    ├── 02cec7a4ef7e5c1a7c99da1e8187c727412b13d6.nq.gz
    ├── 03d5ea9f7db6138f3b524a91d07e2f745ac73f34.nq.gz
    ├── 0468852675294a811d08ea1964b22ac80203d7a3.nq.gz
    ├── 04cdc013ecfdb34723ca87357bf9504cc026daff.nq.gz
    ├── 05318e415e71b1945c7df984bcc60429a17c5e02.nq.gz
    ├── 058ecd574b74013b23dd0fb09c950ffed717de45.nq.gz
    ├── 0765d3db9032375954b223abce5b913ec2c14249.nq.gz
    ├── 0b08695a1c0c6094c2f2f0e29e5472d47f9d8843.nq.gz
    ├── 0bebd183ec4288c5e2ce4b1b6881730ebbe52324.nq.gz
    ├── 0c03efe97da7fdcdf459f333b3a7826174a5d1b7.nq.gz
    ├── 0c7269fd3b250948fa56510a0e422cf6a5b60ed0.nq.gz
    ├── 0ceecc93d5898750c4264a953ed64f1574c14037.nq.gz
    ├── 0da5803d55d3ac6d87b410a1f8556d715f9a93ef.nq.gz
    ├── 0f74c31d9b19455e2891f8f32b0e17f91b1a2376.nq.gz
    ├── 117541837001fff9b586b5db50597c1d93bf1685.nq.gz
    ├── 12eab77a6a7d4b9d47b3297d2a07aedf4edece4d.nq.gz
    ├── 134d01b15a50d093b34681112fadef64e168c8fe.nq.gz
    ├── 1420deaf29db6beaf60bd995ea77b4fd04aa7c72.nq.gz
    ├── 16fe87b06e802f094b3fbb0894b137bca2b16ef1.nq.gz
    ├── 192d1136a2d813b91dfe1627fb0a2576cefa39b9.nq.gz
    ├── 197d4a89377c4dd854db503833b9055c0ccb323e.nq.gz
    ├── 197ec237af7851b36111add4ae1342b00a123fb8.nq.gz
    ├── 1a1186ecbf8338f0e58cccaa4b497f0537f714df.nq.gz
    ├── 1aca557277a292d1b70dc8ad4ebf3d863865a793.nq.gz
    ├── 1bac13ad40876ad23c81e58c6d8bdc283f99e24f.nq.gz
    ├── 1c4cd5ad05be8d5703008b96edc7e56816e8885b.nq.gz
    ├── 1c703f3a40d41080e6b2575d3153e8d11f6b6c78.nq.gz
    ├── 1ca2453721f5105f90c75eb7a306e31de1df6493.nq.gz
    ├── 1d6bfd3a706f6938643e4e7f31177f1ebb2fbf8c.nq.gz
    ├── 1e0c389d2dc99cfeea5a8d42fa2e82720281e4ef.nq.gz
    ├── 1e43e26ba12b7f69ccae669c7288a7deba32a3ad.nq.gz
    ├── 1e4f22bde6a4859bb38ce727f10a3c37ed70b912.nq.gz
    ├── 200d58e08078bb7d08cfd1a4e1791aef472a4455.nq.gz
    ├── 20b9e375e0c8b7b7a94c59a96a9ac56214cd87e4.nq.gz
    ├── 210f53bb5a22bd47ba87acda1d347e4dda7af57d.nq.gz
    ├── 212fa3d42b628a898ec907c0357407e76251eed9.nq.gz
    ├── 21605a91949df6d960f569d346d536ad1125e6ca.nq.gz
    ├── 21abd55d6c16e959313e193d80ca5dbf85dcf122.nq.gz
    ├── 21c1de70f0294e024dc3548e77fbd2f3b2be1ef8.nq.gz
    ├── 222990d2e306cd720d20592a0c40d8848df21587.nq.gz
    ├── 2236bc63f124720b9274592ccecd86bc74582a8a.nq.gz
    ├── 2352a874aca34962910139bdc3fa39d6947f8af0.nq.gz
    ├── 238f85f2ac571ddc51cae84573becc7d1123bfdb.nq.gz
    ├── 23e93fbd0a5f38f746ecf190efaaf1e186e7644b.nq.gz
    ├── 25cefaf52a2a997f15b9ea0dd44bcc98eafe84f4.nq.gz
    ├── 262cb1e72d8c1e76931e763762b29776dcdcce68.nq.gz
    ├── 269780639f34bdefd6101ede2db94ea6af2a4162.nq.gz
    ├── 279b1a3bc7d38ccf50bc85214bcc76c6228fbb5b.nq.gz
    ├── 28d4d768378d68b735784e30c52d5e7c601e1b00.nq.gz
    ├── 28e630cf40d23e85e1b1c48eea4c7c2e8afd90f9.nq.gz
    ├── 2997f8246b778c561f65d8f661df52d96ce85106.nq.gz
    ├── 2a9e296064d298adcdf79cc5dd58a5d490b3aac3.nq.gz
    ├── 2beec8c0c69092651b6130c13c64f19deaed21f8.nq.gz
    ├── 2d63d0dc8fad13d721f5cbfec8f1211bdb8a172b.nq.gz
    ├── 2dccfc779770defa39b3fd855b7ccca6c5871abf.nq.gz
    ├── 31522abae6dc546d5f24eebce5a100305b909110.nq.gz
    ├── 318f35ef333ec7d4aabe6ef9c1cfbf7e142f66c0.nq.gz
    ├── 323e39e108cac98574ad7b34a4e2fc658843ebcd.nq.gz
    ├── 324e7e6c7b7e33a0ba2b6c3ede23a601c0f407cc.nq.gz
    ├── 3290dae4c58889d3fa5daf39432949b281c65719.nq.gz
    ├── 32ec4968e5ae307f0a20a8b8aa095c1c17035341.nq.gz
    ├── 3324f862a990eef96e398c0d100c14c54aa935ef.nq.gz
    ├── 33e36511dabfdb79e21a3101033453921aee0aae.nq.gz
    ├── 3605eba38af9250d651a0e3e353e3497a7fa5eb6.nq.gz
    ├── 37097ca377863483e1323b37a322974b3e8d3863.nq.gz
    ├── 3818c7102b2de3e9d21c50996e97a1d71c2d8f77.nq.gz
    ├── 38369425f2a0f28ead3d445fda9f99fe639b6c3d.nq.gz
    ├── 38c1e27b8e2ead2bb0b2716dc305ed593775935a.nq.gz
    ├── 390202f38b27dcce74a5f5958d61e55e975342fd.nq.gz
    ├── 392300ea905b574fb57f649009189c79c158c1b0.nq.gz
    ├── 3927b25f95c557ac338e946f43a251fa28a29a64.nq.gz
    ├── 398ec11aac705921f8f0e9220339ebe56cafefce.nq.gz
    ├── 3a67db789eb725ce45c83528ff6fa4c50b88f810.nq.gz
    ├── 3ac7f039bc95cfa1eb0426df4f04cf97c6046b0d.nq.gz
    ├── 3ae98e5a0816eea755388edb0acc10ebe63481cd.nq.gz
    ├── 3af7c3beaaba9df8eeef6516c5151bc97f01f182.nq.gz
    ├── 3be5ba3d1a994e05a301891a8e96bc1bfdba27d7.nq.gz
    ├── 3c89b2652405f7eb60998f0ab720ada083dfd35e.nq.gz
    ├── 3dcbb42846f303f77ad71fe93171137283da4a73.nq.gz
    ├── 3e32480673e3ca663c7b65ad27b8be159ba1214f.nq.gz
    ├── 3e6570e2053897e3a0a37b4bf40b2ba23e641a33.nq.gz
    ├── 3ebd1fc708329a00fc357bc2dc45a7ae3331ba30.nq.gz
    ├── 40274185631badf973809243f604b995fa1ed3e9.nq.gz
    ├── 4061533e662f9848fcaba33d7837044ca2515d90.nq.gz
    ├── 40cc9239566c5712919aef42e5fedcaa59b4cba5.nq.gz
    ├── 42630b857b88dd7e8becfbc953349df1ea474836.nq.gz
    ├── 42b0d2982272c93d60c80e868653b22fb376d9ab.nq.gz
    ├── 4373fd1cf53e126dbcd2bd5fc3a4f69c93b3d2b3.nq.gz
    ├── 43eb5ddee10aee60dc43b0aaae2923473fd93699.nq.gz
    ├── 458ee439f66a60f2d074f23dee6749030e026f6f.nq.gz
    ├── 459e7cc1d45470afa5a7a325f570ea616209664c.nq.gz
    ├── 46b0376b587341c8f5da81fb423a28c2a29aaa17.nq.gz
    ├── 491ff56f9400566458292b0956099dcf6360e1ad.nq.gz
    ├── 4c5a96652ece3d787313c1898274ea30471398a4.nq.gz
    ├── 4ccbe34da58615d80c54075a31b115553578643d.nq.gz
    ├── 4d9af8ccfb2346b3fcb9383c4456dc8f47db665f.nq.gz
    ├── 4dbf4544694b46590a4be076c027635e949a5890.nq.gz
    ├── 4ded9ad403a62adfa867a39484dc72a44d5d2edb.nq.gz
    ├── 4e386478ebad2c88c10577d1a3c808f8374ff596.nq.gz
    ├── 4e5dd354d49954caf43889ccf57a3e96880be124.nq.gz
    ├── 4ef02b13d393f9fca7a732478688dbf9398921d8.nq.gz
    ├── 4f278fdd3af8915e565394e4ddc97aa8dc15d232.nq.gz
    ├── 4f9aec2da57d0056a224f2f5bec1f52844bc0a6d.nq.gz
    ├── 4fa5b5cc5cfa9067298082f9bb3930fe62c2de01.nq.gz
    ├── 50b11fbc888eeaa8f5103605705efdf1b0d2d3b2.nq.gz
    ├── 50d650389926d7c93c5c9382195e7a088c6706ce.nq.gz
    ├── 50dfc099965fc5b6022c392be5f2288c0e56498d.nq.gz
    ├── 521118bce6070c5078c7180be9e0a4d3aadbaca0.nq.gz
    ├── 527a6818ce7cb3b915e82d315fc8e8cc94750ef6.nq.gz
    ├── 53de28b33751c59bbe6172d96c4cbf5f2f5702ab.nq.gz
    ├── 546b8c50f3a1b57c1148e276ce6a2792d635db4c.nq.gz
    ├── 54ec202bb1e9fb2c38ff60c3928bde7294b6ae98.nq.gz
    ├── 550d47d9320b5b5e682d73380ec66036752564a2.nq.gz
    ├── 583b615874430d7abbfca1f6b3f8565a4efc59f6.nq.gz
    ├── 59c728e926b03d1d43dc662f899d671b5d7f5f5a.nq.gz
    ├── 59d438b76148e7e700af54f7193c6bf886300c9f.nq.gz
    ├── 5aa73bfb5f479b5cdb045806858eec0bb3f8d539.nq.gz
    ├── 5d5a7e5afe3dd3f4d5468e36a984a281e1b65589.nq.gz
    ├── 5e0a756cb9a0a8e6b31055b318ee219faa3a476c.nq.gz
    ├── 5e5bf2a30e39deb3ca0afdd2aea1d86818c704d2.nq.gz
    ├── 5f8eedeba39b136fb32a749f090c8bdd858ae786.nq.gz
    ├── 5faba6d1771a3ce2833e721f343477889e0a4fd4.nq.gz
    ├── 6036aa997b95ab941a450912f728faee86e6da44.nq.gz
    ├── 614fb50ac3a6817fa751dcbe39014433078a574a.nq.gz
    ├── 6263a1607da997c00a3e655813988c171b632e51.nq.gz
    ├── 62d8da53f608f7131ed8debaa0e499f7c311a3c4.nq.gz
    ├── 63634c82b61728b7f7bfcebc777768fe26ee66f5.nq.gz
    ├── 644d144cf879f6b49f8975f8c85326758e133464.nq.gz
    ├── 6544b738fa248fd755bcc25a88199450ca488ad7.nq.gz
    ├── 65472543c10d9878b23e55df937af324f6d73456.nq.gz
    ├── 65a3f2ddbd09c135595ec5cd2b1123bafdee4775.nq.gz
    ├── 65b1351b9ee688c6214d3a7b9f5cf4fa82282ce4.nq.gz
    ├── 65ba0faccdbd10a5c62d475caa0952d929aa4869.nq.gz
    ├── 65d65eff242bc65576ed8897f8730fb59b55bcba.nq.gz
    ├── 666bf9471ccc2af7ab450467484f57ec6a8794fb.nq.gz
    ├── 6672f07a167bc2097796b85ee95658dbc7ba11e4.nq.gz
    ├── 66d10b9510cf6987f987dfb432914e94aa3d96e0.nq.gz
    ├── 689a6013682a05f6c304642486ca98c3442d384b.nq.gz
    ├── 69b7f463155130761dd81f2c86d6ef7eaeb5100b.nq.gz
    ├── 69c3f079e0f2da3d8dd7613c44e311dd2113aaab.nq.gz
    ├── 6a71bebfe02c120fb65d97b3d74c2cec2cdb4403.nq.gz
    ├── 6b0ffc5ba1534a5fa00405308d2795708af6f7be.nq.gz
    ├── 6b6207b59439a731d6ce668876eae95924f402e3.nq.gz
    ├── 6bc5d49f2c3e2df66c16ec6d0a6c828bf0867d21.nq.gz
    ├── 6c1e164e8a4b22e9f9947eb291faba646bf38104.nq.gz
    ├── 6cbb8cd45c669049320ac80889d07c952b849f08.nq.gz
    ├── 6e55c38ccda70a927557c587741531580b9a09fa.nq.gz
    ├── 6e9d9121fcb30c9468e3eac77eb4526fe14b5d2c.nq.gz
    ├── 6ef3d5e92c5633f19d84af6a6d8136175c89524d.nq.gz
    ├── 7056d5c8cd25eaf3c4f7eceb9d54ccdf3ac1aa65.nq.gz
    ├── 72960fadf2efb3395686913733f9db834b0b7287.nq.gz
    ├── 72a5595d7686d1ab882c6cb7751cb2ce540cbbee.nq.gz
    ├── 72b3af80b9fafed9984eb371ffff4bdf7fe2211e.nq.gz
    ├── 731af300d9f2df65f55fac86684d0cb4c7124181.nq.gz
    ├── 73c982924ecc5bba307f321f269cf890ae4a2ab7.nq.gz
    ├── 74c78cc8025b48e72833539e534ce3edc5bc3bfd.nq.gz
    ├── 756e8ff1bf92dfd98289d65fcbe5a6224d33b25e.nq.gz
    ├── 75ac9b7eb1d5ef7b27a50155e76b57d6f949d995.nq.gz
    ├── 781cc971bf6d2d65f5b38f852d1aa0199044d1df.nq.gz
    ├── 7957f09edd559caf87d5e7b635aa3b9a2a7eee21.nq.gz
    ├── 79810b6a73fc4be71dbe05f875cf0d47f03fc28f.nq.gz
    ├── 7a029aaecac70b395ae2883f06c9999db4270d08.nq.gz
    ├── 7aa9b1d217eaa65fdeb86908b3bf2211e8333455.nq.gz
    ├── 7b3b4bd578580dff3adc134f552a7127a801b789.nq.gz
    ├── 7cc7f8133ba92e616d90b76b259720654d55a4dc.nq.gz
    ├── 7d1e5152aed974119b18739a814ca465a219a3e1.nq.gz
    ├── 7db6414c05c028460fdfaeff1e8239ac361bb1d7.nq.gz
    ├── 7ddbbf37fe66524d6000f71c1e62c2af0ced2b53.nq.gz
    ├── 805229a0e857236812b2daa4c441c28fe5148753.nq.gz
    ├── 8062ca39f16a4dafe8040568ca51479b8ec97db9.nq.gz
    ├── 80d09600ea379dcca2ad1c34df5e741de80a0108.nq.gz
    ├── 814d5843d01c07cd7025a5217d119f28bb90d5e2.nq.gz
    ├── 8155c9d916fbb3f08cb9045feba893c35873cdd3.nq.gz
    ├── 81cc3e5110aa63cc6017e774da3117753ccd97cb.nq.gz
    ├── 81d817a90f43194f05ae2e7a0840a80cd14db320.nq.gz
    ├── 83efa66e58390fc09d7d58223ab741e9417c2a09.nq.gz
    ├── 853ceda5fbdde13681b1bafeda73ccbee565b11b.nq.gz
    ├── 8714da9a51f4f6973d7417f51a449bc4fe71543e.nq.gz
    ├── 88903643ff8e9d3c50e3efafb2e0c2e1a0bad2f7.nq.gz
    ├── 8982ff5a9f8e633e5d452a432f3e32f41a5234ac.nq.gz
    ├── 89cc3d16e0781d42d1153b71a973474d5bed1940.nq.gz
    ├── 8ab144917fe92e63325753f2369ee70e9fd2b7d4.nq.gz
    ├── 8b58c0c204fc1b00ef360402e4c7771034156ed4.nq.gz
    ├── 8ba75092db268e4c82875cd64d74469b0f2dd025.nq.gz
    ├── 8ccdc06a8d5f4b10453bd76feed788d6bac83165.nq.gz
    ├── 8d4915b9d55928139a244a243aa25290cb3363dc.nq.gz
    ├── 8ef6b6959a53a0657c2874071807a16f46f4a0c9.nq.gz
    ├── 9023eec5fbb15f3c970b52b2fa3495b748f2bcba.nq.gz
    ├── 909a4d60b3dae7505b3e275ac48b30032b5c6dd2.nq.gz
    ├── 90bc2c9b75b8554f9eee786fd668fff3399b99f9.nq.gz
    ├── 92097ad9eaf0947ea24bfb4601e8c9b837deb9c5.nq.gz
    ├── 92d65a90ff61202dd3c1bcebf1419828f2a384ee.nq.gz
    └── 942b6a09aeeba233c55c28d9aecd96641d9edfcd.nq.gz

8 directories, 200 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |

## Source repository

[tokio-rs/tokio](https://github.com/tokio-rs/tokio)

---
*Parsed on 2026-05-08 by [repolex](https://repolex.ai)*
