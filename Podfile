# Uncomment the next line to define a global platform for your project
platform :ios, '7.0'

target 'scratch2romo' do
  # Comment the next line if you don't want to use dynamic frameworks
  # use_frameworks!

  # Pods for scratch2romo
  pod 'Romo'
  pod 'Romo/RMCharacter'
  pod 'CocoaAsyncSocket'

  target 'scratch2romoTests' do
    inherit! :search_paths
    # Pods for testing
  end

end

post_install do |installer|
    installer.pods_project.targets.each do |target|
        target.build_configurations.each do |config|
            config.build_settings['BITCODE_GENERATION_MODE'] = 'bitcode'
            config.build_settings['ENABLE_BITCODE'] = 'YES'
        end
    end
end