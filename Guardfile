guard 'bundler', :notify => false do
  watch('Gemfile')
end

group 'server' do
  guard 'rails', :force_run => true do
    watch('Gemfile.lock')
    watch(%r{^(config|lib)/.*})
  end
end
