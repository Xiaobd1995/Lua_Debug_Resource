# Lua_Debug_Resource
lua script debugging resource for the ssRender Editor

lua脚本里在调试的时候需要加上以下三行：
1、告诉lua去哪加载luasocket动态库：
package.cpath = "D:/workspace/ssRenderEditor/Projects/Project1909/resource/luaScript/?.dll;" .. package.cpath
2、告诉lua去哪加载LuaPanda.lua：
package.path = "D:/workspace/ssRenderEditor/Projects/Project1909/resource/luaScript/?.lua;" .. package.path
3、启动LuaPanda文件：
require("LuaPanda").start("127.0.0.1", 8818);
