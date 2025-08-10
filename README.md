local keys = {  -- Add as many key
    "QBwbpfFaGuwXYDNUfWvwvXKqCTueimLN", 
    "zTpouetOhhyYDkoZNZGURxmabaHbyRsM",
    "GenPsKiukCHlxYIpekFmSbuXmOTIWPcE",
    "wKCkGlDdcBdjjevSvaXOznWcgokMzjty",
    "xgPWHHtQksXdTPapkGbqOnPuQUPvqWQt",
    "sAIMoWBQZFcgnfTYpkHNUIisbuwYLbja",
    "ACmMvuDSkcXWHHhyhIvkoudfzPLlWBih",
    "kDszvcQZRaxbRiJJSqNSixWVHLPanlvT",
    "MwTlAebUxgcutQSOjyIroFnEkgtLIhVW",
    "DbynOVdlLOrjMoYQfEyspIEIIqeJihKD",
    "eEpuHPgQGmPvIqZreZdTUyYueWbpyHIt",
    "QqicoaRWKnTLJVqxGPtjHRjzYCRpkrql",
    "GkILBjixsBvuZUIGPMsupvJBQuvGxxJu",
    "gwLvRdBEqmfpILMmboHrRHHWNkRLuhGO",
    "AIbgAOBRNUVpJMHgFVDgVWkzUMITJdBE",
    "TSRdpxTjiRhlYCreVQKiRZmJakInuvME",
    "dQtuQkKJNqsJkHudcsYPeHHIxIUKbFAJ",
    "tAWZlmcBbNlIeVawDjFlSSYgKWKCcFAp",
    "UTLmFeaHnnBmIdZlXvohuHiNfxrUSNTG",     
}

script_key = keys[math.random(#keys)];
setfpscap(2)

getgenv().gagConfig = {
    -- Event:
    CRAFT_EVENT = { "Anti Bee Egg" },
    BUY_TRAVELING_MERCHANT = { "Bee Egg", "Loquat", "Feijoa", "Pitcher Plant" },
    MAX_EVENT_RESTOCK_SHECKLES = 32896000000,
    CLAIM_FOOD_CONNOISSEUR_REWARD = { "Culinarian Chest", "Gorilla Chef", "Gourmet Egg", "Sunny-Side Chicken", "Pet Shard Aromatic", "Cooking Cauldron", "Gourmet Seed Pack", "Bitter Melon Seed", "Pricklefruit Seed", "Butternut Squash Seed", "Spring Onion Seed", "Kitchen Crate", "Kitchen Flooring", "Kitchen Cart", "Smoothie Fountain" },
    
    -- General:
    AUTO_UPDATE_RESTART = true,
    REDEEM_CODES = {},
    EXTRA_PET_SLOTS = 5,
    EXTRA_EGG_SLOTS = 5,
    ADD_FRIEND = true,
    OPEN_ALL_SEED_PACK = true,

    MAX_PLANTS = 250,
    DESTROY_UNTIL_MIN_PLANTS = 200,
    DELETE_PLANTS_AFTER_MAX = { "Carrot", "Strawberry", "Blueberry", "Tomato", "Apple" },
    LIMIT_PLANT_SEED = { ["Strawberry"] = 5, ["Blueberry"] = 5, ["Apple"] = 5, ["Tomato"] = 5, ["Corn"] = 5, ["Bamboo"] = 5, ["Coconut"] = 5, ["Pumpkin"] = 5, ["Watermelon"] = 5, ["Pepper"] = 5 },
    
    BUY_EGGS = { "Bug Egg", "Bee Egg", "Paradise Egg", "Mythical Egg", "Common Summer Egg", "Rare Egg", "Uncommon Egg" },
    PLANT_EGGS = { "Gourmet Egg", "Corrupted Zen Egg", "Zen Egg", "Dinosaur Egg", "Primal Egg", "Anti Bee Egg", "Bee Egg", "Night Egg", "Bug Egg", "Paradise Egg", "Mythical Egg", "Common Summer Egg", "Rare Egg", "Uncommon Egg" },
    
    BUY_SEED_SHOP = { "Elder Strawberry", "Giant Pinecone", "Burning Bud", "Sugar Apple", "Ember Lily", "Beanstalk", "Cacao", "Pepper", "Mushroom", "Grape", "Mango", "Dragon Fruit", "Cactus", ["Coconut"] = 50, ["Bamboo"] = 50, ["Apple"] = 50, ["Pumpkin"] = 50, ["Watermelon"] = 50, ["Daffodil"] = 50, ["Tomato"] = 50, ["Orange Tulip"] = 50, ["Blueberry"] = 50, ["Strawberry"] = 50, ["Carrot"] = 50 },
    KEEP_SEEDS = { "Bone Blossom" },
    KEEP_SEEDS_AFTER_MAX_PLANTS = { "Carrot" },
    
    FAVOURITE_FRUIT_MUTATIONS = {},  -- Stop Autosell
    SKIP_HARVEST_MUTATIONS = {},  -- Stop Harvest

    KEEP_PETS = { "Junkbot", "Gorilla Chef", "Lobster Thermidor", "French Fry Ferret", "Corrupted Kitsune", "Raiju", "Mizuchi", "Kitsune", "Bald Eagle", "Spinosaurus", "Brontosaurus", "T-Rex", "Fennec Fox", "Disco Bee", "Raccoon", "Queen Bee", "Night Owl", "Dragonfly", "Butterfly", "Mimic Octopus", "Red Fox", "Sushi Bear", "Pack Bee", "Petal Bee", "Bear Bee", "Hamster", "Blood Owl", "Cooked Owl", "Golden Bee", "Spaghetti Sloth", "Firefly", "Chicken Zombie", ["Kodama"] = 6, ["Corrupted Kodama"] = 6, ["Blood Kiwi"] = 2, ["Capybara"] = 1, ["Starfish"] = 2, ["Chicken"] = 2, ["Rooster"] = 2, ["Tanchozuru"] = 2, ["Kappa"] = 1 },
    KEEP_PETS_WEIGHT = {},
    KEEP_PETS_AGE = {},

    -- EQUIP_PETS Priority (Left -> Right)
    EQUIP_PETS = { ["Spaghetti Sloth"] = 2, ["Capybara"] = 1, ["Sushi Bear"] = 2, ["Starfish"] = 1, "Gorilla Chef" },
    USE_PETS_FOR_UPGRADE_SLOT = { "Starfish" },
    REMOVE_PET_MAX_UPGRADE = { "Capybara", "Starfish" },

    BUY_GEAR_SHOP = { "Master Sprinkler", "Godly Sprinkler", "Advanced Sprinkler", "Basic Sprinkler" },
    USE_SPRINKLER = { "Basic Sprinkler", "Master Sprinkler", "Godly Sprinkler", "Advanced Sprinkler" },

    PET_WEBHOOK_URL = "https://discordapp.com/api/webhooks/1399625532022456421/DMrHZBfzCP2iZhH7AAiP8DTnPYauCI2UEblNX9__FUgoav03MHwFW5Tsz0GQ8FpPEn-m",
    SEED_WEBHOOK_URL = "https://discordapp.com/api/webhooks/1399625532022456421/DMrHZBfzCP2iZhH7AAiP8DTnPYauCI2UEblNX9__FUgoav03MHwFW5Tsz0GQ8FpPEn-m", 
    NOTIFY_PETS = { "Lobster Thermidor", "French Fry Ferret", "Corrupted Kitsune", "Kitsune", "Fennec Fox", "Disco Bee", "Raccoon", "Queen Bee", "Night Owl", "Dragonfly", "Butterfly", "Mimic Octopus", "Brontosaurus", "T-Rex", "Spinosaurus" },
    NOTIFY_PETS_WEIGHT = {},
    DISCORD_ID = "833710279103217754",
    WEBHOOK_NOTE = "Fus",
    SHOW_WEBHOOK_USERNAME = true,
    SHOW_WEBHOOK_JOBID = true,
}

loadstring(game:HttpGet("https://api.luarmor.net/files/v3/loaders/6cb882027ef5de19462b160764dcfb53.lua"))()
