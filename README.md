# 区块链API网关 (AllOrigins版)

这是一个极简版的区块链API网关，使用AllOrigins作为代理服务来绕过CORS限制。所有API密钥和端点都直接硬编码在HTML文件中。

## 特点

- **单文件部署** - 整个项目只有一个HTML文件
- **无需后端** - 使用AllOrigins作为代理，不需要自己的服务器
- **零配置** - 所有API密钥和端点已硬编码
- **可静态托管** - 可以部署在任何静态网站托管服务上

## 支持的区块链网络

- 以太坊 (eth)
- Polygon (polygon)
- Arbitrum (arbitrum)
- Optimism (optimism)
- Gnosis (gnosis)
- Blast (blast)
- Avalanche (avalanche)
- Scroll (scroll)

## 支持的API

1. **区块链RPC API** - 各大公链的JSON-RPC接口
2. **1inch API** - DEX聚合器API
3. **Reservoir API** - NFT市场数据API
4. **CCXT (模拟)** - 加密货币交易所API（基于公共REST接口模拟）
5. **WalletConnect** - Web3钱包连接

## 部署说明

1. 直接将`index.html`文件上传到任何静态网站托管服务，如GitHub Pages、Netlify、Vercel等
2. 无需任何额外设置，页面就可以直接使用

## 使用方法

页面提供以下功能：

1. **区块链RPC API** - 向各区块链网络发送JSON-RPC请求
2. **1inch API** - 查询1inch交易聚合器API
3. **Reservoir API** - 查询NFT市场数据
4. **CCXT** - 查询各大交易所的行情数据
5. **WalletConnect配置** - 获取WalletConnect配置信息

## API密钥信息

- **区块链RPC节点** - Ankr API密钥
- **WalletConnect项目ID** - `64b6a6cc7a2296ccb0b97b887b6dee1a`
- **1inch API密钥** - `BFmmhv1wAlc12w1jd6xy8YMy5y0sxLPh`
- **Reservoir API密钥** - `d1d6d023-5e2f-5561-8184-6417a48c2f01`

## 注意事项

- 由于使用AllOrigins作为代理，API请求可能会受到AllOrigins服务限制
- POST请求通过AllOrigins可能不总是可靠，具体取决于AllOrigins的支持情况
- 所有API密钥都是公开的，请勿用于敏感操作 