task default: %w[publish]

task :publish do
  system('git add -u')
  system('git add .')
  message = "Site updated at #{Time.now.utc}"
  system('git commit -m #{message.inspect}')
  system('git commit -m "commit by rakefile"')
  system('git push')
end