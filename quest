-- Created by Thalles Vitor --
-- Quest Chest --
local storage = 4400 -- storage of quest, add +1 to others quests
local itemlist = {2160, 2148} -- items id list
local itemlist_count = {1, 2} -- count of items list

function onUse(cid, item)
   if getPlayerStorageValue(cid, storage) >= 1 then
      doPlayerSendTextMessage(cid, 25, "It's empty.")
      return true
   end

   -- Player Gain The Items (ITEMLIST)
   for i = 1, #itemlist do
      doPlayerAddItem(cid, itemlist[i], itemlist_count[i])
   end

   doPlayerSendTextMessage(cid, 25, "Quest done!")
   setPlayerStorageValue(cid, storage, 1)
   return true
end
