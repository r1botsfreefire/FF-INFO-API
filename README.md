# 📝 API Documentation

##  Account Information API
API Route = https://wlx-demon-info.vercel.app/profile_info?uid={uid}&region={region}


### 📨 Request Example
```http
GET https://wlx-demon-info.vercel.app/profile_info?uid=12022250&region=ind
```

### ☑️ Query Parameters

| Parameter | Type   | Required | Description                   |
|-----------|--------|----------|-------------------------------|
| `region`  | string | Yes      | The region code (`sg`, `ind`, `br`,`id`, `tw`, `us`, `sac`, `th`, `me`, `pk`, `cis`, `bd`).|
| `uid`     | int | Yes      | The user ID.                  |
| `key`     | string | No      | Join https://t.me/FFwlx_demon.                  |


📚 **Purpose of the API**  

The primary purpose of providing this free API is to enhance the Free Fire community experience. Garena Free Fire does not offer official account information APIs, so this custom solution aims to fill that gap, providing players and developers with valuable account data


🧩 **(Some of🤫) Frameworks and Libraries Used**  
- **Flask**: A micro web framework for Python to build the API endpoints.
- **Flask-CORS**: For handling Cross-Origin Resource Sharing (CORS).
- **PyCryptodome**: For implementing Decryption and Encryption.
- **Requests**: For making HTTP Requests to Server.

# 📁 Additional Information

- This API response Does not Represent the Actual Structure Received from the Official Garena Server.
- The Response structure is simplified in an User-Friendly Structure for the ease of understanding for Anyone at any level of Programming.
- All images related to item IDs shown by the API response (e.g., avatars, banners, outfits, weapons) are available at `https://freefiresite.vercel.app/icon?item={itemID}` for the convenience of API users in their development projects.


### 💬 Example of a Successful Reponse May Look Like this,
```json
{
  "AccountInfo": {
    "AccountAvatarId": 902000013,
    "AccountBPBadges": 6,
    "AccountBPID": 1001000081,
    "AccountBannerId": 901000021,
    "AccountCreateTime": 1512554331,
    "AccountEXP": 4916417,
    "AccountLastLogin": 1738757394,
    "AccountLevel": 76,
    "AccountLikes": 1081046,
    "AccountName": "RaiㅤStarㅤ모",
    "AccountRegion": "IND",
    "AccountSeasonId": 43,
    "AccountType": 1,
    "BrMaxRank": 206,
    "BrRankPoint": 1550,
    "CsMaxRank": 212,
    "CsRankPoint": 43,
    "EquippedWeapon": [912034001],
    "ReleaseVersion": "OB47",
    "Role": 2,
    "ShowBrRank": true,
    "ShowCsRank": true,
    "Title": 904090027
  },
  "AccountProfileInfo": {
    "EquippedOutfit": [211000045, 205000590, 203001250, 211000303, 204000077, 214000000],
    "EquippedSkills": [16, 5801, 8, 1, 16, 6501, 8, 2, 16, 3206, 8, 3, 16, 1706]
  },
  "GuildInfo": {
    "GuildCapacity": 55,
    "GuildID": "61575940",
    "GuildLevel": 6,
    "GuildMember": 37,
    "GuildName": "RAIㅤBR0THERS",
    "GuildOwner": "12022250"
  },
  "api dev": "@wlx_demon",
  "captainBasicInfo": {
    "EquippedWeapon": [912034001],
    "accountId": "12022250",
    "accountType": 1,
    "badgeCnt": 6,
    "badgeId": "1001000081",
    "bannerId": "901000021",
    "createAt": "1512554331",
    "csMaxRank": 212,
    "csRank": 212,
    "csRankingPoints": 43,
    "exp": 4916417,
    "headPic": "902000013",
    "lastLoginAt": "1738757394",
    "level": 76,
    "liked": 1081046,
    "maxRank": 206,
    "nickname": "RaiㅤStarㅤ모",
    "rank": 206,
    "rankingPoints": 1550,
    "region": "IND",
    "releaseVersion": "OB47",
    "seasonId": 43,
    "showBrRank": true,
    "showCsRank": true,
    "title": 904090027
  },
  "creditScoreInfo": {
    "creditScore": 100,
    "periodicSummaryEndTime": "1739054110",
    "periodicSummaryStartTime": "1738794910",
    "rewardState": 1
  },
  "petInfo": {
    "exp": 3001,
    "id": 1300000001,
    "isSelected": true,
    "level": 6,
    "name": "Kitty",
    "selectedSkillId": 1315000002,
    "skinId": 1310000003
  },
  "socialinfo": {
    "AccountLanguage": "Language_English",
    "AccountPreferMode": "Prefermode_BR",
    "AccountSignature": "oh ok"
  },
  "success": true
}

```
# 😵 Error Responses
API might Show Error Response Upon Users' Inaccurate Requests!

### Error Instances and Solutions

- **Error Code:** 400
  - **Message:** Invalid region.
  - **Solution:** Make sure you are using a valid region code.

- **Error Code:** 429
  - **Message:** Abnormal Requests Detected. Please Avoid Misusing Info API for Visits or Your IP may get Blocked!
  - **Solution:** Avoid excessive requests or contact the API provider for assistance.

- **Error Code:** 500
  - **Message:** An error occurred while processing your request. Please Recheck Your ID & Region.
  - **Solution:** Double-check the provided user ID and region, and retry the request. If the issue persists, contact the API provider for support.

---

API Made By WLX DEMON,
All Rights Reserved!