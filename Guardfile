require "coffee_script"
require "eco"

notification :growl

guard :sprockets, :destination => "/Volumes/Projects/jmseg-pricing/Pricing/Cotador/Content/js/", :asset_paths => ["../jmseg-pricing/Pricing/Cotador/Content/assets/templates", "../jmseg-pricing/Pricing/Cotador/Content/assets/javascripts"] do
  watch (%r{Pricing/Cotador/Content/assets/.*}) do |m|
    "application.js"
  end
end

guard :sprockets, :destination => "/Volumes/Projects/jmseg-pricing/Pricing/Pricing/Content/js/", :asset_paths => ["../jmseg-pricing/Pricing/Pricing/Content/assets/templates", "../jmseg-pricing/Pricing/Pricing/Content/assets/javascripts"] do
  watch (%r{Pricing/Pricing/Content/assets/.*}) do |m|
    "application.js"
  end
end