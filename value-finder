if gg.isVisible(true) 
  then 
    gg.setVisible(false)
  end

function main()
Menu = gg.choice({"Float Value Search","Dword Value Search","Qword Value Search","Word Value Search","Search Ranges","Exit"}, nil,"Value Finder Script")

if Menu == 1 then F1() end
if Menu == 2 then F2() end
if Menu == 3 then F3() end
if Menu == 4 then F4() end
if Menu == 5 then F5() end
if Menu == 6 then Exit() end
end

function F1()
  p = gg.prompt({"Enter Value","Change Value"})
  gg.searchNumber(p[1],gg.TYPE_FLOAT)
  r = gg.prompt({"Enter Refine Number"})
  gg.refineNumber(r[1])
  gg.getResults("5000")
  gg.editAll(p[2],gg.TYPE_FLOAT)
gg.toast("Completed Search .... Changed Value")
end

function F2()
  p = gg.prompt({"Enter Value","Change Value"})
  gg.searchNumber(p[1],gg.TYPE_DWORD)
  r = gg.prompt({"Enter Refine Number"})
  gg.refineNumber(r[1])
  gg.getResults("5000")
  gg.editAll(p[2],gg.TYPE_DWORD)
gg.toast("Completed Search .... Changed Value")
end

function F3()
  p = gg.prompt({"Enter Value","Change Value"})
  gg.searchNumber(p[1],gg.TYPE_QWORD)
  r = gg.prompt({"Enter Refine Number"})
  gg.refineNumber(r[1])
  gg.getResults("5000")
  gg.editAll(p[2],gg.TYPE_QWORD)
gg.toast("Completed Search .... Changed Value")
end

function F4()
  p = gg.prompt({"Enter Value","Change Value"})
  gg.searchNumber(p[1],gg.TYPE_WORD)
  r = gg.prompt({"Enter Refine Number"})
  gg.refineNumber(r[1])
  gg.getResults("5000")
  gg.editAll(p[2],gg.TYPE_WORD)
gg.toast("Completed Search .... Changed Value")
end


function F5()
Menu = gg.choice({"Region Anonymous","Region Video","Region C_BSS","Region Code App","Region C Alloc","Back"}, nil,"GG Ranges")

if Menu == 1 then G1() end
if Menu == 2 then G2() end
if Menu == 3 then G3() end
if Menu == 4 then G4() end
if Menu == 5 then G5() end
if Menu == 6 then main()end
end

function G1()
gg.setRanges(gg.REGION_ANONYMOUS)
gg.toast("TRUE")
end

function G2()
gg.setRanges(gg.REGION_VIDEO)
gg.toast("TRUE")
end

function G3()
gg.setRanges(gg.REGION_C_BSS)
gg.toast("TRUE")
end

function G4()
gg.setRanges(gg.REGION_CODE_APP)
gg.toast("TRUE")
end

function G5()
 gg.setRanges(gg.REGION_C_ALLOC)
gg.toast("TRUE")
end
function Exit()
gg.clearResults()
os.exit()
end

main()

while(true)
do
  while gg.isVisible(true)
    do
      gg.setVisible(false)
      main()
    end
end
