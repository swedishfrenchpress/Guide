---
layout: guide
title: overview
description: A primer on ecash on bitcoin
nav_order: 1
parent: ecash
grand_parent: How it works
permalink: /guide/how-it-works/ecash/overview
redirect_from:
 - /guide/ecash/overview/
main_classes: -no-top-padding -ecash-page
image: https://bitcoin.design/assets/images/guide/how-it-works/ecash/ecash.jpg
---

{% include picture.html
   image = "/assets/images/guide/how-it-works/ecash/ecash.jpg"
   retina = "/assets/images/guide/how-it-works/ecash/ecash@2x.jpg"
   mobile = "/assets/images/guide/how-it-works/ecash/ecash-mobile.jpg"
   mobileRetina = "/assets/images/guide/how-it-works/ecash/ecash-mobile@2x.jpg"
   alt-text = "ecash overview illustration"
   width = 1600
   height = 700
   layout = "full-width"
%}

<!--

Editor's notes

Figma file: https://www.figma.com/file/ZwRT4mZZ4UNGtsfLz22m8M/Liquidity?node-id=0%3A1
Figma file for channel reserve UI's: https://www.figma.com/file/6iJpftEbajA3y1ylXQxsrl/Channel-reserve

-->

# Ecash
{:.no_toc}

---

<div class="glossary-toc" markdown="1">
* Table of contents
{:toc}
</div>

---
## What is ecash?

Ecash is a digital payment system that uses cryptographic techniques to ensure secure and private transactions. Developed by David Chaum in 1933, it operates through a mint that issues digital tokens in exchange for deposited funds. These tokens can be spent and received without revealing user identities or transaction details, thanks to blinded signatures. Users can redeem their tokens for the original funds at any time. Since no accounts or personal information are needed; the mint cannot see your balance, tokens, or transaction details, offering a highly private and efficient method for digital payments.

### How does ecash on bitcoin work?

Ecash on Bitcoin works by integrating the principles of Chaumian ecash with the Bitcoin network, utilizing the Lightning Network for efficient transactions.

* **Mint Creation** - A mint is established by an individual or organization. This mint is responsible for issuing eCash tokens, which represent Bitcoin.

* **Depositing Bitcoin** - Users deposit Bitcoin into the mint. In return, the mint issues eCash tokens that are equivalent to the deposited Bitcoin amount.

* **Blinded Signatures** - To enhance privacy, the mint uses blinded signatures. This cryptographic technique ensures that the mint cannot trace the tokens it issues back to the individual users.

* **Spending ecash** - Users can spend their ecash tokens with merchants or other users. They can also send transactions over the Lightning Network.

* **Receiving ecash** - Recipients of eCash can store these tokens in their ecash wallets. The tokens can be used for further transactions or eventually redeemed for Bitcoin.

* **Redeeming ecash** - When users want to convert their ecash tokens back into Bitcoin, they can redeem the tokens at the mint. The mint verifies the tokens and transfers the equivalent amount of Bitcoin to the user.

{% include tip/open.html color="blue" icon="info" label="Ecash tip" %}

Insert important key insight about ecash here.

{% include tip/close.html %}

## Advantages of ecash for Bitcoin

Ecash on Bitcoin offers several significant advantages:

{% include tip/open.html color="blue" icon="info" label="Ecash tip" %}

Include an illustration to help make it easier for a user to follow along.

{% include tip/close.html %}

* **Enhanced Privacy** - ecash uses blinded signatures, ensuring that transaction details, including user identities and amounts, remain hidden. This level of privacy is superior to traditional Bitcoin transactions.

* **Speed** -Since transactions are processed by a centralized mint ecash transactions are fast and efficient, which helps in handling a large volume of transactions without the limitations that exist on bitcoin on-chain or the Lightning Network.

* **Low Costs** - The processing of ecash transactions is inexpensive, making it a cost-effective solution for both small and large payments.

* **Ease of Use** - Users do not need to manage complex aspects of the Bitcoin, such as channels or liquidity, simplifying the user experience.

* **Flexible Mint Options** - Multiple independent mints can operate, allowing users to choose mints based on their reputation, fees, and other preferences. This decentralization reduces reliance on a single entity.

**Reduced Trust Assumptions** - While users deposit funds with a mint, the design minimizes the level of trust required compared to traditional custodial wallets. The mint does not have access to user transaction data or balances.

## Ecash compared to custodial lightning

{% include tip/open.html color="blue" icon="info" label="Ecash tip" %}

Include a graphic that compares ecash to custodial lightning.

{% include tip/close.html %}

The Problems With Custodial Lightning

<div class="nodes -full-width" markdown="1">
   <table>
      <thead>
         <tr>
            <th>&nbsp;</th>
            <th>
               {% include picture.html
                  image = "/assets/images/guide/how-it-works/liquidity/node-rachel.png"
                  retina = "/assets/images/guide/how-it-works/liquidity/node-rachel@2x.png"
                  alt-text = "Depiction of Rachel and a dedicated hardware lightning node"
                  width = 236
                  height = 236
               %}
               Ecash
            </th>
            <th>
               {% include picture.html
                  image = "/assets/images/guide/how-it-works/liquidity/node-miguel.png"
                  retina = "/assets/images/guide/how-it-works/liquidity/node-miguel@2x.png"
                  alt-text = "Depiction of Miguel and a cloud lightning node"
                  width = 236
                  height = 236
               %}
               Custodial Lightning
            </th>
         </tr>
      </thead>
      <tbody>
         <tr>
            <td>Privacy</td>
            <td>Example</td>
            <td>Example</td>
         </tr>
         <tr>
            <td>Censorship resistence</td>
            <td>Example</td>
            <td>Example</td>
         </tr>
         <tr>
            <td>Rugability</td>
            <td>Example</td>
            <td>Example</td>
         </tr>
      </tbody>
   </table>
</div>

As you can see Ecash helps improve on Custodial Lightning.