# LibMemoize
Adapting kikito's memoize.lua library (https://github.com/kikito/memoize.lua) for World of Warcraft

Usage:

	local function MyFunc(foo, bar, ...)
	    ...
	end
	local cache = {};
	local memoize = LibStub("LibMemoize-2.0");

	local MyMemoizedFunc = memoize.memoize(MyFunc, cache);
