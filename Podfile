# Uncomment the next line to define a global platform for your project
# platform :ios, '9.0'

target 'SBIM' do
  # Comment the next line if you don't want to use dynamic frameworks
  use_frameworks!

  # Pods for SBIM
  pod 'DropDown', '~> 2.3.3'
  target 'SBIMTests' do
    inherit! :search_paths
    # Pods for testing
  end

  target 'SBIMUITests' do
    # Pods for testing

  end

end
post_install do |pi|
  pi.pods_project.targets.each do |t|
    t.build_configurations.each do |config|
      config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '15.0'
    end