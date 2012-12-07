require "coffee_script"
require "eco"

notification :terminal_notifier_guard

guard :sprockets, :destination => "/Volumes/Projects/jmseg-pricing/Cotador/Content/js/", :asset_paths => ["../jmseg-pricing/Cotador/Content/assets/templates", "../jmseg-pricing/Cotador/Content/assets/javascripts"] do
  watch (%r{Cotador/Content/assets/.*}) do |m|
    "application.js"
  end
end

guard :sprockets, :destination => "/Volumes/Projects/jmseg-pricing/Pricing/Content/js/", :asset_paths => ["../jmseg-pricing/Pricing/Content/assets/templates", "../jmseg-pricing/Pricing/Content/assets/javascripts"] do
  watch (%r{Pricing/Content/assets/.*}) do |m|
    "application.js"
  end
end