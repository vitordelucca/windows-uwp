---author: payzer
title: Device Portal SMB API reference
description: Learn how to access the SMB APIs programatically.
ms.author: wdg-dev-content
ms.date: 02/08/2017
ms.topic: article
ms.prod: windows
ms.technology: uwp
keywords: windows 10, uwp
ms.assetid: 1f0eb76e-fe3e-4674-a27e-229beec7e63d
---# Developer folder API reference   You can access development-related files on your Xbox One using a standard file explorer. This allows you to easily view and replace files from your PC to the console.**Request**You can access the developer folder using the following request. The request will return:    * The location of the file share. This location can be entered into the address bar in a file explorer.* The username to access the file share.* The password to access the file share.Method      | Request URI:------     | :-----GET | /ext/smb/developerfolder<br />**URI parameters**- None**Request headers**- None**Request body**- None**Response**   Path - the path to the file developer files share.   Username - the username needed to access the developer files share.   Password - the password needed to access the developer files share.   **Status code**This API has the following expected status codes.HTTP status code      | Description:------     | :-----200 | The request to access the credentials for the file share was granted.4XX | Error codes5XX | Error codes<br />**Available device families*** Windows Xbox