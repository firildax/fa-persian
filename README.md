# سالیدیتی زبان برنامه نویسی قرارداد گرا

شما می توانید از طریق [![solidity at https://gitter.im/ethereum/solidity](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/ethereum/solidity?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) سوالات، باز خورد ها و پیشنهادات خودتان را با ما در میان بگذارید!

سالیدتی یک زبان سطح بالا ی قرارداد گرا با نوع نوشتار ثابتی است که برای ساختن قرارداد های هوشمند در پلتفرم اتریوم استفاده می شود.

## فهرست

- [مثال](#مثال)
- [نحوه ساخت محلی مستندات](#نحوه-ساخت-محلی-مستندات)
- [مثال](#مثال)
- [مستندات](#مستندات)
- [نگهدارنده ها](#نگهدارنده-ها)

## نحوه ساخت محلی مستندات

1. ابتدا یک محیط مجازی در `Python3` می سازیم و وارد پوشه محیط مجازی می شویم:

```bash
virtualenv solidity-doc
cd solidity-doc
```

2. سپس با استفاده از دستور زیر محیط مجازی را فعال می کنیم:

```bash
source bin/activate
```

3. سپس مخزن مستندات فارسی سالیدیتی را از اینجا بر می داریم و وارد پوشه می شویم:

```bash
git clone https://github.com/firildax/fa-persian
cd fa-persian
```

4. لیست وابستگی های مورد نیاز در فایل `requirements.txt` قرار دارند با دستور زیر تمام آنها را نصب می کنیم

```bash
pip install -r requirements.txt
```

5. سپس وارد پوشه مستندات شده و دستور ساخت فایل های `html` را صادر می کنیم:

```bash
cd /docs
make html
```

اسناد سالیدتی در مسیر زیر در دسترس شما هستند:

`_build/html/index.html`

## مثال

یک برنامه "سلام دنیا!" که در بیشتر زبان های برنامه نویسی دیگر مورد استقبال نیست. اما اینجا هست:

```solidity
// SPDX-License-Identifier: MIT
pragma solidity >=0.6.0 <0.9.0;

contract HelloWorld {
    function helloWorld() external pure returns (string memory) {
        return "Hello, World!";
    }
}
```

برا شروع سالیدیتی شما می توانید از [Remix](https://remix.ethereum.org/) استفاده کنید
که یک IDE تحت وب است. اینجا چند مثال تقدیم می شود:

1. [Voting](https://docs.soliditylang.org/en/latest/solidity-by-example.html#voting)
2. [Blind Auction](https://docs.soliditylang.org/en/latest/solidity-by-example.html#blind-auction)
3. [Safe remote purchase](https://docs.soliditylang.org/en/latest/solidity-by-example.html#safe-remote-purchase)
4. [Micropayment Channel](https://docs.soliditylang.org/en/latest/solidity-by-example.html#micropayment-channel)

## مستندات

اینجا مستندات سالیدیتی به انگلیسی قرار دارد [Read the docs](https://docs.soliditylang.org).

## نگهدارنده ها

- [@axic](https://github.com/axic)
- [@chriseth](https://github.com/chriseth)

## نگهدارنده بخش فارسی

- [@saracodic](https://github.com/saracodic) سارا

## کوچیک شما

- [@firildax](https://github.com/firildax) آرمین
