---
ROBOTS: NOINDEX,NOFOLLOW
title: "Add bot to Telephony"
description: "Enable your bot to interact with users directly over the phone."
ms.date: 05/10/2022
ms.topic: article
author: v-alarioza
ms.author: v-alarioza
manager: shellyha
ms.reviewer: mivakoc
ms.custom: "publication, ceX"
ms.collection: virtual-agent
---

# Add bot to Telephony

[!INCLUDE [Build 2022](includes/build-22-disclaimer.md)]

Connect your [Azure Communication Service (ACS)](/azure/communication-services/) phone number to enable your bot to interact with users directly over the phone.

## Prerequisites

- [Publishing fundamentals](publication-fundamentals-publish-channels.md)

## Connect your bot to Telephony

1. In the side navigation under **Settings**, select **Channels**.

1. Select the **Telephony (Preview)** tile.

    :::image type="content" source="media/publication-connect-bot-to-telephony/telephony-tile.png" alt-text="Screenshot of Telephony tile.":::

1. Select **Connect existing phone number**.

1. Choose an **Azure Subscription** and **Azure Communication Services resource**, then select **Select**.

    :::image type="content" source="media/publication-connect-bot-to-telephony/choose-resources.png" alt-text="Screenshot of selected Azure resources.":::

1. For **Phone number type** choose **PTSN**.

    > [!IMPORTANT]
    > The **Direct routing** option is not supported in the technology preview.

1. Under **PTSN phone numbers** select the first number in the list, then select **Connect**.

    > [!IMPORTANT]
    > Phone numbers have been been provisioned for the technology preview, but normally you'll need to do this yourself in ACS.

    :::image type="content" source="media/publication-connect-bot-to-telephony/connect-number.png" alt-text="Screenshot of selected phone number.":::

1. Once the connection is ready, [publish your bot](publication-fundamentals-publish-channels.md#publish-the-latest-bot-content) and test it by calling the number you selected.

To further customize how your bot speaks, learn [how to use Speech Synthesis Markup Language](advanced-custom-speech-ssml.md) and [change your bot's voice font](advanced-speech-settings.md).

## Disconnect your bot from Telephony

Only one bot can be connected to a phone number. If you want to connect a different bot, you'll first need to disconnect the old bot.

1. In the side navigation under **Settings**, select **Channels**.

1. Select the **Telephony (Preview)** tile.

    :::image type="content" source="media/publication-connect-bot-to-telephony/telephony-tile.png" alt-text="Screenshot of Telephony tile in channel list.":::

1. Select **Disconnect**.

    :::image type="content" source="media/publication-connect-bot-to-telephony/disconnect-bot.png" alt-text="Screenshot of disconnect button.":::
