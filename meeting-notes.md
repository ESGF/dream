---
layout: default
title: Meeting Notes
---

<script type='text/javascript' src='http://ajax.googleapis.com/ajax/libs/jquery/1.10.1/jquery.min.js'></script>  
<script type="text/javascript" src="{{ site.baseurl }}/Data/media/js/simpleJekyllSearch.js"></script>
<div id="content" class="column">
<div class="section">
    <a id="main-content"></a>
    <h1 class="title page-heading" id="page-title">
        Meeting Notes        
    </h1>
    <div class="home">
        <div class="well well-lg">
            <div id="form-group">
                <input type="text" id="search-input" class="form-control" placeholder="Search..." >
                <ul id="results-container"></ul>
            </div>
        </div>
        <div class="alert alert-warning" role="alert">
            Search box only searches the questions and tags, not the anwser text. To do a full body search please use your browser search <kbd><kbd>ctrl</kbd> + <kbd>F</kbd></kbd> or <kbd><kbd>command</kbd> + <kbd>F</kbd></kbd>  
        </div>
        <div class="region region-content">
            <div id="block-system-main" class="block block-system">
                <div class="content">
                    <div id="node-14" class="node node-book node-full clearfix" about="/content/meeting-notes" typeof="sioc:Item foaf:Document">
                        <span property="dc:title" content="Meeting Notes" class="rdf-meta element-hidden"></span><span property="sioc:num_replies" content="0" datatype="xsd:integer" class="rdf-meta element-hidden"></span>
                        <div class="content clearfix">
                            <div id="book-navigation-14">
                                <ul class="menu clearfix">
                                    <div class="list-groups">
                                        {% for post in site.posts %}
                                        <div class="list-group-item">
                                            <h2><a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h2>
                                            <p>{{ post.content }}</p>
                                        </div>
                                        {% endfor %}
                                    </div>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>
<script type="text/javascript">
    SimpleJekyllSearch.init({
      searchInput: document.getElementById('search-input'),
      resultsContainer: document.getElementById('results-container'),
      dataSource: '{{site.baseurl}}/search.json',
      searchResultTemplate: '<li><a href="{{site.baseurl}}/{url}" title="{desc}">{title}</a></li>',
      noResultsText: 'No results found',
      limit: 10,
      fuzzy: false,
    })
</script>
<style type="text/css">
    #search-demo-container {
    max-width: 40em;
    padding: 1em;
    margin: 1em auto;
    border: 1px solid lightgrey;
    }
    #search-input {
    display: inline-block;
    padding: .5em;
    width: 100%;
    font-size: 0.8em;
    height: 34px;
    -webkit-box-sizing: border-box;
    -moz-box-sizing: border-box;
    box-sizing: border-box;
    }
    .post-header {
        display: none;
    }
    .book-navigation{
        display: none;
    }
</style>