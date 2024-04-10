
## Проверка на принадлежность к пакету протокола FTM
```C
static inline bool ieee80211_is_ftm(struct sk_buff *skb)
{
	struct ieee80211_mgmt *mgmt = (void *)skb->data;

	if (!ieee80211_is_public_action((void *)mgmt, skb->len))
		return false;

	if (mgmt->u.action.u.ftm.action_code ==
		WLAN_PUB_ACTION_FTM_RESPONSE &&
	    skb->len >= offsetofend(typeof(*mgmt), u.action.u.ftm))
		return true;

	return false;
}
```