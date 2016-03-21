if File.exists?("./config.rb")
  # Compile on start.
  puts `compass compile --time --quiet`
  # https://github.com/guard/guard-compass
  guard :compass do
    watch(%r{(.*)\.s[ac]ss$})
  end
end

# Compress JS
guard :jammit, :output_folder => "scripts/js/min/" do
  watch(%r{^scripts/(.*)\.js$})
end

# Example copy and rename to liquid-ize a compiled asset
# guard :copy3, from: 'scripts/js/min/application.js', to: 'scripts/js/min/application.js.liquid', rename: true

guard 'livereload' do
  watch(%r{.+\.(html|liquid)$})
  watch(%r{styles/.+\.(css|js|html)})
  watch(%r{scripts/js/min/.+\.(css|js|html)})
end
