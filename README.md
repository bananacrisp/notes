notes
=====

post '/groups' do
    group = Group.create(:group_name => params['add_group'], :url => params['add_group'].gsub(' ', "_"))

    redirect "/groups/#{group.url}"
  end
