# Repolex Knowledge Graph of pytorch/text

RDF knowledge graph data for [pytorch/text](https://github.com/pytorch/text), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download pytorch/text
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── a5e610638ea47b4412a29cdb708ac5f2fabb1286
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── a5e610638ea47b4412a29cdb708ac5f2fabb1286
│           └── chunk-001.nq.gz
└── blob
    ├── 0023a687b3d4d0b795a5e97cc914bdabb5a253df.nq.gz
    ├── 00ea624bdf7222e0ca5695cff614298e7d3a9602.nq.gz
    ├── 01810aa5c27950bee2862cf9d1d0ce668fd7513e.nq.gz
    ├── 0288a564e22755147c1daf1cfec1db59fcc998c9.nq.gz
    ├── 02b0b45339e092eb0d2e24220c07a270b6a34014.nq.gz
    ├── 079025ca62f9d69be05b952f40c269b92583ed13.nq.gz
    ├── 08559f0c6874cda75e630221cf88dfb94d4ecbe0.nq.gz
    ├── 0949eb103c8524689c9f8dcb2a5d973aa3dd7966.nq.gz
    ├── 0ac313115d899d57cac07ab081f3defc3523eef9.nq.gz
    ├── 0ac7bd8fb650e9e1881be3c7f86ada55ae290d84.nq.gz
    ├── 0ad1e25ac1134ab2ac10380f9b57f76834ab83f2.nq.gz
    ├── 0b6c9aa6660be1b73d4510b95c215a7d29eea4ba.nq.gz
    ├── 0bacca430c3f270b61a57c402480f8d662eff40a.nq.gz
    ├── 0c7e28c3b35489872d3425dc7cbe511911140cbc.nq.gz
    ├── 0cacb02c6b50c97852bc8fe6ca4a51d928023eb3.nq.gz
    ├── 0db91e67534ce19b76dc774a99f4de8d89d0a344.nq.gz
    ├── 0df74a4b391de12315d28678ba020540a8ed0567.nq.gz
    ├── 0f7cf2920f5a26fd12cc34bcb010bd49ab70c190.nq.gz
    ├── 0fa3ae2b005d0d1a39e9e841403cd6284914f9ce.nq.gz
    ├── 119cb62e696772a9bc37f2a1ef792690d8c35804.nq.gz
    ├── 130f14a094ad1d8d93480de91989e00da5e6a4f0.nq.gz
    ├── 1344c4673710e402a942fec1321ec7e034e2e83f.nq.gz
    ├── 13b0c6ecad9a3a447e8ecc8cfd35378d1d02304e.nq.gz
    ├── 13ed4a480bc32c25c7fa5a3676af026017401efc.nq.gz
    ├── 15e9bbc0469f57221c9996a5d2a9d93618a8dcc7.nq.gz
    ├── 1738aa3e528b2acffad59a5684a81dfbf462ffcc.nq.gz
    ├── 174bee75664ce27e36f197ada3db78cf836c14ca.nq.gz
    ├── 18789c5dcda98dffec1cfbdf4f0da3b44252ef0e.nq.gz
    ├── 1bcb2f73e76ed47e4fed649b46e9d8cc05f7c53b.nq.gz
    ├── 1e1d0e0502da9df68d54e60a139f3b25511e9826.nq.gz
    ├── 1f66bf5279b6e158eca8588deaf927ed4a75c9ab.nq.gz
    ├── 1fd0de3014b07e2ed4c099fd5f238509b5818ac3.nq.gz
    ├── 2095647fe43a4f429e63842994b318ceab3e2699.nq.gz
    ├── 21053a31f0fb7e4f0b6f8e4ea8949314f8b82093.nq.gz
    ├── 21400cdde00cf41a0c4600b6cedffb2387f97ae6.nq.gz
    ├── 2195b0a748ba57340289c063ef69a6db05ef031e.nq.gz
    ├── 221e1d639acf87bb39c2d78a3a57b5862774ce63.nq.gz
    ├── 2242588d1ee576160ceab6f598efc71441a4e4a6.nq.gz
    ├── 226b0752cac7789c48f0cb3ec53eda48b7be36cc.nq.gz
    ├── 22a57a492a9c211f6e538155f622fcf06ba5ede1.nq.gz
    ├── 22c3398f5109385cddaf830b11e345034befd862.nq.gz
    ├── 24418bd27c7b8e2c57c4c53fd88f6bfab0c2e5ae.nq.gz
    ├── 27c8693a5c8d0fa9fc08317d907d4fdd4f935492.nq.gz
    ├── 2928abba1859f8c6ae2a4ea9485628b2acf74a9c.nq.gz
    ├── 296970ea086443f3645df1d399f7c28f6d086f58.nq.gz
    ├── 2b658efcfb6888782af407f5e4262b79093432c0.nq.gz
    ├── 2c001cc26584417395efca0974fce5e933eb989c.nq.gz
    ├── 2c904e7f03dce94a0cddc53d0dc5e01f36a6ec9b.nq.gz
    ├── 2d7b1fac445c8042ed87dcdbdfbe57520cc2e1c7.nq.gz
    ├── 2ea941cc79a6f3d7985ca6991ef4f67dad62af04.nq.gz
    ├── 2ec49c1d73656c3dea76e388cb7ede35e4dcf0c8.nq.gz
    ├── 2f02a6cb6cdb8ef0e630e1da8edd53d699929f40.nq.gz
    ├── 2f49308fc7bd164a8b6238e9ad050483807ad235.nq.gz
    ├── 33ac388bc4a99bc63ab1b8b9e5514d6d82d42192.nq.gz
    ├── 358052ec012940bb56778d167bcd69302d255846.nq.gz
    ├── 361435f43da43f7245c38f8cab7ecafd3adeeec6.nq.gz
    ├── 36fa8e99c92d9993b0352cd1b463702ef752ef1e.nq.gz
    ├── 370633f2ec2b7cf35a37a283095229de337f46e4.nq.gz
    ├── 373f3378099d52222fab5a2303f5d91d425bcf0d.nq.gz
    ├── 3743207557dd9f8b065f4a4d580091e7a4476824.nq.gz
    ├── 37dd43a5bd25da76fed31939995fc3572120006c.nq.gz
    ├── 3b28b078645500d6c24aafb7dd05573228fe50a8.nq.gz
    ├── 3b44c3af62a0472431f87b767978d0e02eb56e91.nq.gz
    ├── 440e811ce4fbc7cf2814a4590be9ec6d5aa0349f.nq.gz
    ├── 44abb5403cca4dde9885620608fe4529d852b931.nq.gz
    ├── 4595627b50d9751e90f8688caa64ddd031be2b39.nq.gz
    ├── 45d955c0b91323f291adf6a6ac839c4d63d2a36b.nq.gz
    ├── 48ba29d91410be3238d8e73cd1301866190a5c41.nq.gz
    ├── 4a62ae2400fc169b65a9ebf12224f56c6d63c86c.nq.gz
    ├── 4b8923423a9c844779e1aabd58e8c78f51f1b142.nq.gz
    ├── 4ce3481105a2d643eb3e933ce276c394cc679815.nq.gz
    ├── 4e28ff6ebdf584f5372d9de68867399142435d9a.nq.gz
    ├── 4e4bb23987dd58c8b1fba91891c3ecb8e81f3624.nq.gz
    ├── 4e651145cc7f060d7b7178658e25001ce427f0d5.nq.gz
    ├── 4fff9354a9e8f0c47ff0792f0d4c9b6739bdd0f7.nq.gz
    ├── 500d0ba2a960073281554a6cdb2779b875d6e06d.nq.gz
    ├── 5411765c99d05de99d4658c4e5046c13c47f3325.nq.gz
    ├── 565fb5a1ac928ad60b468583cea0738add8334b1.nq.gz
    ├── 5777e638f1607c189191cb945286a0d20118f273.nq.gz
    ├── 5781f6f86ef5c867d6e20236600f0eaf852aaa27.nq.gz
    ├── 5789499927f3a916e20525d8a7099540d724d208.nq.gz
    ├── 5888eb54b1accd0f7a5be03990d96e5321546a3e.nq.gz
    ├── 58d579716a4116df124f4b617914abb8dbb908a3.nq.gz
    ├── 58faf6e6344ae5a47df35b34f47477f534227189.nq.gz
    ├── 5aaa9249988ef68e188ee8f82c4c8ccb8bfd5733.nq.gz
    ├── 5acf8bcc8a642c5637d19b777c2b11c10ffd4c46.nq.gz
    ├── 5b10fe4a737ec196b42a97dcc38d147b5a606365.nq.gz
    ├── 5c263d8c93b17d413e32cd700756a5c2630ea480.nq.gz
    ├── 5c61b2519e04617b3f7aedc8600c350579e27d39.nq.gz
    ├── 5d67bba8adc4abd2b1b1f11d24c1695a1a092151.nq.gz
    ├── 5dc54aa1168232d7408b32632d3344ec0967b1cb.nq.gz
    ├── 5ee238473138e856ef09c26e8e54bebedef3a49d.nq.gz
    ├── 5f2fb76be77348f13d8d016a7514dd9b03e9cc8c.nq.gz
    ├── 5f6e85180fd0e744a8473dae0a66c722629ff517.nq.gz
    ├── 5f8c695b508e5fe3740c40cefe71c469149cda8a.nq.gz
    ├── 6023169ac17a8c3028fc89f05a2fd515e2ad8359.nq.gz
    ├── 603fcb98c1a5fc395f86484a695541cba4822999.nq.gz
    ├── 6052ad08b106accec140ef3f0e27cb4fe893377a.nq.gz
    ├── 60f0a04c071478a7c4c6732877573cb7a2e74616.nq.gz
    ├── 61915a1790b095f92cd353cb2c3abde56c568210.nq.gz
    ├── 61c1612a91eb7c56869df0f551fc9fd9fda3a7b1.nq.gz
    ├── 638d3ca7f55dd40a65315fc43a384f768b3d9122.nq.gz
    ├── 6396ddc813dc90b07a0146f53596c04d72921838.nq.gz
    ├── 641bffd61aed9264179ceb2f30cb952aefa293d7.nq.gz
    ├── 64ade31c6c39079c5702d974817f67814aa573ac.nq.gz
    ├── 65c2188d871044ba233a158f2c43bc417d977192.nq.gz
    ├── 670d9bc4a5a5bdea7e62f543b34c39405ecfa0eb.nq.gz
    ├── 685e08bb589dd34a433da0e07a163283171b1957.nq.gz
    ├── 6a2989cd6c3aa2d0bcd5c31fb26c02b1c700d6b6.nq.gz
    ├── 6a858773fcc913cb0574af372d5280a450297ecd.nq.gz
    ├── 6b3dbf0f5bcea01e614b44e9e8361496164f1898.nq.gz
    ├── 6ba6debc921d74326cdf165ecded3e552acf0ba4.nq.gz
    ├── 6baff13ad67ca225c27244ca1ae68bc25ace4093.nq.gz
    ├── 6c4d01001529ea9e78bc075f263734250eb54214.nq.gz
    ├── 6e80a7de5e675dab17f1ac1e45cf562ca2e8fb50.nq.gz
    ├── 6ea3ef86a87970a16ac5eeda6729341ec629f493.nq.gz
    ├── 6ec6cd8b29d3fdd3c5826e7ac3befe8551307a1c.nq.gz
    ├── 6f130f81c9e48e7a976cc71f3676611a78888309.nq.gz
    ├── 6f13bcb04434b293a1341e29bdba62bbaa7808a1.nq.gz
    ├── 6f607ba7518e2346e16489195fcdbd111320996c.nq.gz
    ├── 6fa713a5130b8fac749cc4d94e270ffa27eced4c.nq.gz
    ├── 704f676618059d1fbf1f94e5099b50f45b4b8277.nq.gz
    ├── 717a3ce942f8915a8ace66a0b4b78f2e2f6177ca.nq.gz
    ├── 71c637435e10470945f99030fcef6ef2f6fb0037.nq.gz
    ├── 726032fae51926ca49bd54b4cb98957a5dca30e2.nq.gz
    ├── 73fa794117e10a0a79b9a3b284f6b1c7f9099924.nq.gz
    ├── 74126636a57224878f7453f6e7e2567ce78e6d2f.nq.gz
    ├── 748711bed6329dede5d3f1d055b1edcbc1adcf40.nq.gz
    ├── 753dd0716081609b1e58aa7f53535e18d4bf7f40.nq.gz
    ├── 75c8e3e4f3b6a0cf34279b023c53bc2ff6078cc3.nq.gz
    ├── 760b3bb79817b417c62395d7c00af17169506c94.nq.gz
    ├── 762f2f26a0227e1958b9b47bb3c1de342ee0eeab.nq.gz
    ├── 768ce4bb202c2f621fefe78d8a8dc65b32295228.nq.gz
    ├── 76952232aa8c7193ae3e3c78412b01702ef54ecc.nq.gz
    ├── 7806595e679fff1d205b0050abb58c7333af2372.nq.gz
    ├── 7afa3f31cd7a6a999cc0a1b939a1fe61c2647dbd.nq.gz
    ├── 7b3ebe2fe30c204ef19a603acb2e255861769b83.nq.gz
    ├── 7bb96c7ba9e756956d90ad077b67b45c5af4f082.nq.gz
    ├── 7bea8f1211f970fa6b317c1bdeee1ab0aacbaa26.nq.gz
    ├── 7c1db211f43b6c09046fdc9016063c4c59b0e931.nq.gz
    ├── 7c6b579f6f38d5ec798f17d78a1a0dacc184c127.nq.gz
    ├── 7d3afe26a9f5fc5c9c79465ae7e1b55924d94585.nq.gz
    ├── 7eb4810408ce849fb212a5a8715f9680a276b34e.nq.gz
    ├── 7f342b0afde2b58ea8c1cac4d1f2d238a94d2bac.nq.gz
    ├── 80549735e1ce2df3266a4a622a207753d890228e.nq.gz
    ├── 80a0659f98ef0770fd5e7351a7997ffcff136dc7.nq.gz
    ├── 8145b704d1b34982fdc1d7ba0847d0b4ccac7969.nq.gz
    ├── 82566e591deb5f12d04e3924ca9994080ee7dada.nq.gz
    ├── 8645068d3f630330e13f81abfb2647bb40f3c006.nq.gz
    ├── 875fa1b3cf565f6429b0aca71c4c84e4cdd85b53.nq.gz
    ├── 87b0eb2cf7ac0ce81d93f65fbc79a0aee3d99742.nq.gz
    ├── 887675cfdebd7187185d309f372006e9da36774b.nq.gz
    ├── 897174d7fd22b4bf48427b8d8b60c630d1ec476b.nq.gz
    ├── 89a72ea4554061c5f3a29eedb062544b73918e51.nq.gz
    ├── 8a942d9fac0d560b01be4ac507e667a3f9eff06c.nq.gz
    ├── 8b30cc4da812d561a05c325ae828bac618caec8e.nq.gz
    ├── 8b61eefeaa7923a041382dd928f2f4a717bd2fce.nq.gz
    ├── 8c10579fadc10ac0676ff6afdbf5869b3da8dc51.nq.gz
    ├── 8d7de4d6fc31da0d8217381ea7693e370fa9d053.nq.gz
    ├── 8d982f29f0e976311486262ef5c018af905722d4.nq.gz
    ├── 8dd36b91fba151a52e0b7908cdb3973164861053.nq.gz
    ├── 8deed46f4e5452ac9f2aa97e5e85330f5adc5ef9.nq.gz
    ├── 8e6163288c0ec3c714a1ebc564617937506ad097.nq.gz
    ├── 8e860bb5d02edf616221816c44e8b4c72fbaaa48.nq.gz
    ├── 9084dac1a3e872fe4059b90b4d3162ea097521e3.nq.gz
    ├── 915dc4e71f9daf58584453ca18fe5915c491a455.nq.gz
    ├── 92168cf371ec704bff72e7bf6b6dc55f70b8bb95.nq.gz
    ├── 9340649dfe860bd65c549d54295069f986b86a04.nq.gz
    ├── 93ef7fe163492e529a4ec5c079f0f3ce826fcfe3.nq.gz
    ├── 93f398329cae551d7f6331b63ac33143c42bfaba.nq.gz
    ├── 9400308196bb95fff15707f33df7674ea75ce582.nq.gz
    ├── 9410135677a4fdc1113d96c5a422583992c688c3.nq.gz
    ├── 94a0ed4db3eb4bdf2dc59b9144bcdf4ade0b75d5.nq.gz
    ├── 94e90f20310eb517cadcd3d25a8ed21238fd2df5.nq.gz
    ├── 95059c639985d7132676b154bbe43411bb174826.nq.gz
    ├── 9553d884630291346c2a895e3b37213a04666af9.nq.gz
    ├── 95e4bbfad3bb576961f4d0ba1e711cfbad644c36.nq.gz
    ├── 96f3d96abaa49928b850dbca7089138b77ed2149.nq.gz
    ├── 97c2922103e71f9accfe100f04d8000201568fa0.nq.gz
    ├── 983059faf1506e9bef225fe9c07be168bb68fae9.nq.gz
    ├── 9882cb1b258e57ebf1a571a2da91e3b69b09d904.nq.gz
    ├── 996cee6d99680038b180e875ac80723d847cefcc.nq.gz
    ├── 99fff110c2ec1cb35c0eebfd9ed9b1070b419f43.nq.gz
    ├── 9a89ac9b145db031dda15897ffab58a5d0e65da9.nq.gz
    ├── 9c1e53f8b0d7587c57e835d850be549b37680005.nq.gz
    ├── 9d7502200d39897dab7c6e269bafab9f6e73ad4b.nq.gz
    ├── 9dd6e86000a03374ecf4bd47420605072b7e5ca6.nq.gz
    ├── 9e60ccfd2dcb3b43cdd5a64c09029f753ca41e07.nq.gz
    ├── 9ece559d048d9f3d0b2c757c6df1f92bc5b91239.nq.gz
    ├── 9f5287ca3fad00f9fea2608b7c102bdcaca0d204.nq.gz
    ├── a0ab93a23a48113c8050b066b2a2464bdfc0cc56.nq.gz
    ├── a0ed0c6c40df3f94df3c3beca2f1fd36c5b38a35.nq.gz
    ├── a0f177f55d33a966bb817fdcc4c52b5b0cfcfce6.nq.gz
    ├── a14cf457094277d3a2cdfa9aa7b6d4cc05428e8e.nq.gz
    ├── a2640ee4471d2705dbec8a1f790f74ee881b4a57.nq.gz
    ├── a3d3a58e18323dc2f62dfd65645f28a7606ba278.nq.gz
    ├── a4827ca5f446c579d80f32a50af078853ec7f926.nq.gz
    └── a4bc40d68b73002e3be1d5bb5b42bf57a7329e61.nq.gz

7 directories, 200 files
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
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[pytorch/text](https://github.com/pytorch/text)

---
*Parsed on 2026-11-06 by [repolex](https://repolex.ai)*
