Драйвер iwlwifi (intel)

Точка входа [***iwl-drv.c***](https://github.com/torvalds/linux/blob/20cb38a7af88dc40095da7c2c9094da3873fea23/drivers/net/wireless/intel/iwlwifi/iwl-drv.c)

функция ***iwl_mvm_ftm_start***([ftm-initiator.c](https://github.com/torvalds/linux/blob/master/drivers/net/wireless/intel/iwlwifi/mvm/ftm-initiator.c#L906)) вызывается в функции ***iwl_mvm_start_pmsr** ([mac80211.c](https://github.com/torvalds/linux/blob/master/drivers/net/wireless/intel/iwlwifi/mvm/mac80211.c#L6181)) (старт пассивного сканирования радиосреды)
Далее все функции оперделены в [функциональной таблице](https://github.com/torvalds/linux/blob/master/drivers/net/wireless/intel/iwlwifi/mvm/mac80211.c#L6207)