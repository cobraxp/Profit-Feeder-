{
  "General": {
    "BaAseCurrency": "ETH", // MARKET
    "BuyStrategy": "EMASPREAD", // ALL_buy_strategy
    "BuyValue": "-1.45", // ALL_buy_value
	  "BuyValueLimit": "0", // ALL_buy_value_limit used for SPREAD and CROSS strategies only
    "Cost": "0.030", // ALL_max_cost or or All_max_cost_percentage
    "DcaEnabled": "-2", // ALL_DCA_enabled
    "DcaMaxBuySpread": "2", // max_buy_spread in DCA.properties
    "DcaMaxBuyTimes": "2", // max_buy_times in DCA.properties
    "DcaMaxCost": "0", // max_cost in DCA.properties
    "DcaMinBuyBalance": "0", // min_buy_balance in DCA.properties depending on UseMinBuyBalancePercentage in hostsettings.json
    "DcaSellTrigger": "1", // sell_trigger in DCA.properties
    "DcaSellStrategy": "GAIN", // sell_strategy in DCA.properties
    "DcaSellValue": "1", // sell_value in DCA.properties
    "DcaTrailingBuy": "0.077", // trailing_buy in DCA.properties
    "DcaTrailingProfit": "0.117", // trialing_profit in DCA.properties
    "ExcludedPairs": "BNB,BTG,BCD,BLZ,BCPT,IOST,ELF,VIB,LEND,ICN,AE,ADX,AMB,ARN,APPC,CMT,CHAT,CDT,CND,CTR,DLT,DNT,ENG,ENJ,EVX,FUEL,GTO,GVT,GXS,INS,KNC,MANA,MCO,MDA,MOD,MTH,NEBL,OAX,OST,PPT,RCN,RLC,SNM,SNT,TNB,TNT,TRIG,VIA,VIBE,WABI,XZC,YOYO,ZRX", // coins you don't want PTF to create settings for. These will have no config generated and will appear in watchmode
    "SomOnlyPairs": "BTG,BCD,TRIG,MTL,SWIFT,ARDR,SAFEX,BTA,DAR,DRACO,SLING,CRYPT,DOGE,UNO,SC,INCNT,NAUT,SJCX,NOTE,TKN,TIME,BLZ,APPC,GXS", // these are coins where BASE_COIN_sell_only_mode will be true
    "DcaExcluded": "BNB", // coins you don't want DCA enabled for no matter what
	  "EnabledPairsOnly": "", // coins that you only want to trade. If pairs are in here and the ExcludedList, they will not be traded
    "MaxBuySpread": ".75", // All_max_buy_spread
    "MaxTrailingBuy": "0.215", // All_trailing_buy
    "MaxTrailingProfit": "0.215", // All_tailing_profit
    "MinBuyBalance": "0.001", // All_min_buy_balance or All_min_buy_balance_percentage
    "MinBuyPrice": "0.000004", // All_min_buy_price
    "MinBuyVolume": "300", // All_min_buy_volume
    "MinProfit": "1.3", // All_min_profit
    "MinTrailingBuy": "0.097", // minumum the trailing buy after offsets can be
    "MinTrailingProfit": "0.0197", // minumum the trailing buy after offsets can be
    "MinutesForLongerTermTrend": "1440", // minutes to measure trend for LongerTermPriceChange
    "MinutesToMeasureTrend": "30", // minutes to measure trend for base coin trend, PriceTrendChange and volatility calc
    "NumberOfPairs": "10", // ALL_max_trading_pairs
    "SellStrategy": "GAIN", // ALL_sell_strategy
    "SellValue": "1", // ALL_sell_value
    "TopCurrenciesToCheck": "50" // number of pairs to check from your exchange for MaxTopCoinAverageChange
 },
  "MarketConditions": {
    "Configs": [
      {
        "FolderName": "01-superbear",
		"MaxTopCoinAverageChange": "-3",
        "SellOnlyMode": "true",
		"DcaEnabled": "false"
      },
      {
        "FolderName": "02-bear",
		"MaxTopCoinAverageChange": "-1"
      },
      {
        "FolderName": "03-boring",
		"MaxTopCoinAverageChange": "0"
      },
      {
        "FolderName": "04-bull",
		"MaxTopCoinAverageChange": "3"
      },
      {
        "FolderName": "05-superbull",
		"MaxTopCoinAverageChange": "10000"
      }
    ]
  },
   "PriceTrendChange": {
    "Configs": [
	  {
        "MaxPriceTrendPercentageChange": "-10000"
	  },
      {
		"MaxPriceTrendPercentageChange": "-5",
        "TrailingProfitOffset": "-10",
		"DcaEnabled": "false",
		"SellOnlyMode": "true"
      },
      {
        "MaxPriceTrendPercentageChange": "-2",
        "TrailingProfitOffset": "-10"
      },
      {
	    "MaxPriceTrendPercentageChange": "5"
	  },
      {
        "MaxPriceTrendPercentageChange": "15000",
        "TrailingProfitOffset": "-10",
        "SellValueOffset": "-30",
        "SellOnlyMode": "true"	
      }
    ]
  },
  "LongerTermPriceChange": {
    "Configs": [
      {
	    "MaxPriceTrendPercentageChange": "-10000"
	  },
      {
	    "MaxPriceTrendPercentageChange": "-15",
		"TrailingProfitOffset": "-10",
		"SellOnlyMode": "true"
	  },
      {
        "MaxPriceTrendPercentageChange": "10"
      },
      {
        "MaxPriceTrendPercentageChange": "10000",
        "TrailingProfitOffset": "-10",
        "SellOnlyMode": "true"
      }
    ]
  }
 }  
