# Jeeves-Zones-Error
This Error Spamms every tick fills the server log makes it 10 mb big in like seconds.


STACK TRACE
-----------------------------------------
	Lua((MOD:Jeeve's Zones)).pcall(JeevesZonesServer.lua:1142)
	Lua((MOD:Jeeve's Zones)).enforceZedStats(JeevesZonesServer.lua:1142)
	Lua((MOD:Jeeve's Zones)).applyZedPostSpawn(JeevesZonesServer.lua:1311)
	Lua((MOD:Jeeve's Zones)).spawnZedsInZone(JeevesZonesServer.lua:1352)
	Lua((MOD:Jeeve's Zones)).zombiePump(JeevesZonesServer.lua:1451)
	Lua((MOD:Jeeve's Zones)).onTick(JeevesZonesServer.lua:1516)
ERROR: General      f:121 st:53,133,788,484> Lua((MOD:Jeeve's Zones)).pcall> Exception thrown
	java.lang.RuntimeException: attempted index of non-table at KahluaUtil.fail(KahluaUtil.java:100).
	Stack trace:
		se.krka.kahlua.vm.KahluaUtil.fail(KahluaUtil.java:100)
		se.krka.kahlua.vm.KahluaUtil.luaAssert(KahluaUtil.java:90)
		se.krka.kahlua.vm.KahluaThread.tableSet(KahluaThread.java:1474)
		Lua((MOD:Jeeve's Zones)).pcall(JeevesZonesServer.lua:1142)
		Lua((MOD:Jeeve's Zones)).enforceZedStats(JeevesZonesServer.lua:1142)
		Lua((MOD:Jeeve's Zones)).applyZedPostSpawn(JeevesZonesServer.lua:1311)
		Lua((MOD:Jeeve's Zones)).spawnZedsInZone(JeevesZonesServer.lua:1352)
		Lua((MOD:Jeeve's Zones)).zombiePump(JeevesZonesServer.lua:1451)
		Lua((MOD:Jeeve's Zones)).onTick(JeevesZonesServer.lua:1516)
		se.krka.kahlua.vm.KahluaThread.luaMainloop(KahluaThread.java:435)
		se.krka.kahlua.vm.KahluaThread.call(KahluaThread.java:161)
		se.krka.kahlua.vm.KahluaThread.pcall(KahluaThread.java:1749)
		se.krka.kahlua.stdlib.BaseLib.pcall(BaseLib.java:313)
		se.krka.kahlua.stdlib.BaseLib.call(BaseLib.java:111)
		se.krka.kahlua.vm.KahluaThread.callJava(KahluaThread.java:177)
		se.krka.kahlua.vm.KahluaThread.luaMainloop(KahluaThread.java:794)
		se.krka.kahlua.vm.KahluaThread.call(KahluaThread.java:161)
		se.krka.kahlua.vm.KahluaThread.pcall(KahluaThread.java:1749)
		se.krka.kahlua.vm.KahluaThread.pcallvoid(KahluaThread.java:1581)
		se.krka.kahlua.integration.LuaCaller.pcallvoid(LuaCaller.java:60)
		se.krka.kahlua.integration.LuaCaller.protectedCallVoid(LuaCaller.java:131)
		zombie.Lua.Event.trigger(Event.java:55)
		zombie.Lua.LuaEventManager.triggerEvent(LuaEventManager.java:279)
		zombie.gameStates.IngameState.onTick(IngameState.java:1600)
		zombie.gameStates.IngameState.updateInternal(IngameState.java:1514)
		zombie.gameStates.IngameState.update(IngameState.java:1311)
    zombie.network.GameServer.main(GameServer.java:1019)
ERROR: General      f:121 st:53,133,788,484 at KahluaThread.flushErrorMessage      > dumping Lua stack trace

