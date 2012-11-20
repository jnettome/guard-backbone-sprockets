notification :terminal_notifier_guard

guard :shell do
  watch %r{Pricing/Cotador/Content/assets/.+\.(eco|js|coffee)} do |m|
    compile = system('sprockets -I../jmseg-pricing/Pricing/Cotador/Content/assets/javascripts -I../jmseg-pricing/Pricing/Cotador/Content/assets/templates ../jmseg-pricing/Pricing/Cotador/Content/assets/javascripts/application.js.coffee > ../jmseg-pricing/Pricing/Cotador/Content/js/application.js')
    move = system('cp ../jmseg-pricing/Pricing/Cotador/Content/js/application.js /Volumes/Projects/jmseg-pricing/Pricing/Cotador/Content/js/')

    if (compile) && move
      n "Build and move done", "Success", :success
    elsif (compile) && !move
      n "Sorry, I can\'t move application.js", "Error on Move", :warning
    else
      n "See terminal for output", "Error on Build", :failed
    end
  end
end