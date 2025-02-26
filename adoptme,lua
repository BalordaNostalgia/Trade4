-- Create the ScreenGui
local screenGui = Instance.new("ScreenGui")
screenGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")

-- Create the main frame
local mainFrame = Instance.new("Frame")
mainFrame.Size = UDim2.new(0.5, 0, 0.6, 0)
mainFrame.Position = UDim2.new(0.25, 0, 0.2, 0)
mainFrame.BackgroundTransparency = 0.3
mainFrame.BackgroundColor3 = Color3.new(0.1, 0.1, 0.1)
mainFrame.BackgroundTransparency = 0.5
mainFrame.BorderSizePixel = 0
mainFrame.Parent = screenGui

-- Apply UICorner for rounded corners
local corner = Instance.new("UICorner")
corner.CornerRadius = UDim.new(0.1, 0)
corner.Parent = mainFrame

-- Create the show button
local showButton = Instance.new("TextButton")
showButton.Size = UDim2.new(0, 100, 0, 30)
showButton.Position = UDim2.new(0, 10, 0, 10)
showButton.Text = "Show"
showButton.BackgroundTransparency = 0.5
showButton.Parent = mainFrame

-- Create the close button
local closeButton = Instance.new("TextButton")
closeButton.Size = UDim2.new(0, 100, 0, 30)
closeButton.Position = UDim2.new(0, 120, 0, 10)
closeButton.Text = "Close"
closeButton.BackgroundTransparency = 0.5
closeButton.Parent = mainFrame

-- Create the first button
local freezeButton = Instance.new("TextButton")
freezeButton.Size = UDim2.new(0, 200, 0, 50)
freezeButton.Position = UDim2.new(0.5, -100, 0.4, -35)
freezeButton.Text = "Freeze"
freezeButton.BackgroundTransparency = 0.5
freezeButton.Parent = mainFrame

-- Create the second button
local forceAcceptButton = Instance.new("TextButton")
forceAcceptButton.Size = UDim2.new(0, 200, 0, 50)
forceAcceptButton.Position = UDim2.new(0.5, -100, 0.55, -25)
forceAcceptButton.Text = "Force Accept"
forceAcceptButton.BackgroundTransparency = 0.5
forceAcceptButton.Parent = mainFrame

-- Store the original size and position
local originalSize = mainFrame.Size
local originalPosition = mainFrame.Position
local minimized = false

-- Functionality for show button
showButton.MouseButton1Click:Connect(function()
    if minimized then
        mainFrame.Size = originalSize
        mainFrame.Position = originalPosition
        minimized = false
    else
        originalSize = mainFrame.Size
        originalPosition = mainFrame.Position
        mainFrame.Size = UDim2.new(0, 100, 0, 30)
        mainFrame.Position = UDim2.new(0, 10, 0, 10)
        minimized = true
    end
end)

-- Functionality for close button
closeButton.MouseButton1Click:Connect(function()
    screenGui:Destroy()
end)
