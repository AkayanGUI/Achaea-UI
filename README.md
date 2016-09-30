# Achaea-UI
Graphical User Interface for Achaea

gui = gui or { width, height = getMainWindowSize() }

gui.load = function(
  gui = {}
    border = {
      left = { x = 0, y = 0, width = 0, height = 0},
      right = {x = 0, y = 0, width = 0, height = 0}
      top = {x = 0, y = 0, width = 0, height = 0},
      bottom = {x = 0, y = 0, width = 0, height = 0}
    },
  }
}

gui.draw = function()
  for k, v in pairs( gui.border ) do
    gui[k] = Geyser.Label:new({
      name = "gui."..k,
      x = v.x,
      y = v.y,
      width = v.width,
      height = v.height,
    })
    gui[k]:setStyleSheet([[
      background-color: rgba(50,50,50,150);
      border-color: 
    ]])
  end
end

gui.update = function()

end
