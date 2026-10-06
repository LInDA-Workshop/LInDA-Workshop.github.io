---
permalink: /cfp/
title: "Call for Papers"
banner: /images/eacl.png

---
<style>
  html { scroll-behavior: smooth; }
  .page__content h3 { scroll-margin-top: 4em; }

  .sidebar,
  .sidebar.sticky {
    position: relative !important;
    top: 0 !important;
    margin-top: 2em !important;
  }
  .cfp-toc__title { font-weight: bold; margin: 0 0 0.5em 0; }
  .cfp-toc ul { list-style: none; margin: 0; padding: 0; }
  .cfp-toc li { margin: 0.4em 0; }
  .cfp-toc a { text-decoration: none; }
  .cfp-toc a:hover { text-decoration: underline; }
</style>

<p><b>March 13 or 14, 2027 (date to be confirmed) – Hybrid format</b><br>
Co-located with <a href="https://2027.eacl.org/"> EACL 2027</a> in Athens, Greece<br>
Venue: Megaron Athens International Conference Center (MAICC), Room: TBA</p>

<p>LInDA invites papers on the use of linguistic information to improve NLP applications. Each submission must address two points: (1) a linguistic resource or annotation (not necessarily created by the contributors), and (2) its impact on one or more NLP tasks. Papers that cover only one of these points are out of scope.</p>
<h3>Topics of interest</h3><p>Topics include, but are not limited to:</p><ul><li>Leveraging linguistic resources (e.g., annotations, grammars) to improve NLP tasks, particularly for low-resource languages</li><li>Language- and task-specific case studies, as well as more general strategies</li><li>Practical NLP applications, such as tools for second language (L2) learners and for educational purposes, based on linguistically informed material</li><li>Analyzing the quality of linguistic resources (notably, annotation standardization) and their relevance in NLP downstream tasks</li><li>Assessing how linguistic knowledge is represented in pretrained models as a basis for improving their capabilities</li><li>Investigating the language proficiency and metalinguistic skills of language models</li><li>Ethics of data collection, annotation, and NLP tools for underrepresented languages</li><li>Data- and compute-efficient approaches for multi- and mono-lingual modeling, relying on linguistic information for improvement</li><li>Cross-lingual transfer by utilizing linguistic knowledge that supports generalization</li></ul>
<p>Relevant tasks include machine translation, information retrieval, interlinear gloss generation, morphological analysis, parsing, grammatical annotation, and training of language-specific models, among others.</p>

<h3>Paper types</h3>
<p>All accepted papers will be presented as talks or posters.</p>
<p><b>Archival papers.</b> Accepted papers will appear in the workshop proceedings in the ACL Anthology.</p>
<ul><li>Long papers: up to 8 pages of content. They should describe original, completed, and unpublished work. Include evaluation and analysis where possible.</li>
<li>Short papers: up to 4 pages of content. They should present a focused contribution, such as a small experiment, a negative result, a new resource, or an application.</li></ul>
<p>References and appendices do not count toward the page limit. Reviewers are not required to read the appendices. Accepted papers may add one page in the camera-ready version to address the reviews.</p>
<p><b>Non-archival papers</b> <i>(to be confirmed)</i>. Accepted papers will be presented at the workshop but will not appear in the proceedings. This track is open to extended abstracts (up to 2 pages) on ongoing work, and to work already published elsewhere.</p>


<h3>Submission format</h3>
<p>Submissions must follow the two-column ACL format. Please use the official <a href="https://github.com/acl-org/acl-style-files"> ACL LaTeX template</a> (also available on <a href="https://www.overleaf.com/latex/templates/association-for-computational-linguistics-acl-conference/jvxskxpnznfj"> Overleaf</a>). We do not provide a Word template. Submissions must be in PDF.</p>
<p>All papers must include a Limitations section after the conclusion. This section does not count toward the page limit. An Ethical Considerations section is optional and also does not count toward the limit.</p>
<h3>Submission links</h3><p>We use OpenReview for all submissions.</p>
<ul><li>Direct submissions (archival): TBA</li><li>ARR commitment (archival, pre-reviewed papers): TBA</li><li>Non-archival submissions: TBA</li></ul>


<h3>ARR commitment</h3>
<p>LInDA accepts papers that were reviewed through <a href="https://aclrollingreview.org/"> ACL Rolling Review (ARR)</a>. The reviews and meta-review must be available by the ARR commitment deadline. Authors commit their paper through OpenReview. They do not need to change the paper, although they are encouraged to do it for the camera ready following the reviewers' recommendations.</p>

<h3>Multiple submissions</h3>
<p>Following general ACL policy, archival papers must not be under review at another venue during the LInDA review period. We do not accept direct submissions that are under review at ARR, or that overlap with such a submission by more than 25%. Non-archival papers do not have this restriction.</p>
<h3>Double-blind review</h3>
<p>Review is double-blind. Papers must not include author names or affiliations. Cite your own work in the third person ("Smith et al. (2025) showed…", not "We showed…"). Links to code or data must be anonymized. Papers that do not follow these rules may be desk-rejected without review. We follow the <a href="https://www.aclweb.org/adminwiki/index.php/ACL_Policies_for_Review_and_Citation"> ACL Policies for Review and Citation</a>. There is no anonymity period: authors may post preprints during the review period.</p>

{% comment %}
<h3>Presentation</h3>
<p>At least one author of each accepted paper must register for the workshop and present the paper. Remote presentations are possible.</p>
<h3>Best Paper Award</h3>
<p>LInDA will give a Best Paper Award. All accepted archival papers are eligible. A committee of experts will select the winner. The committee will include members of the program committee and external researchers.</p>
<h3>Participation and inclusion</h3>
<p>LInDA is a hybrid workshop. Authors and attendees can take part in person in Athens or online. At least one organizer will be on site and one will be online during the workshop. Online participation will use the EACL 2027 virtual platform.</p>
{% endcomment %}

<p>We encourage submissions from researchers and communities that are underrepresented in NLP, and from authors with diverse backgrounds. We consider both topic fit and diversity in the review and selection process.</p>

<script>
document.addEventListener('DOMContentLoaded', function () {
  var sidebar = document.querySelector('.sidebar');
  var content = document.querySelector('.page__content') || document;
  var heads = content.querySelectorAll('h3');
  if (!sidebar || !heads.length) return;

  var html = '<nav class="cfp-toc"><p class="cfp-toc__title">On this page</p><ul>';
  heads.forEach(function (h, i) {
    if (!h.id) {
      h.id = h.textContent.toLowerCase().replace(/[^a-z0-9]+/g, '-').replace(/^-|-$/g, '') || 'section-' + i;
    }
    html += '<li><a href="#' + h.id + '">' + h.textContent + '</a></li>';
  });
  html += '</ul></nav>';

  sidebar.innerHTML = html;
});
</script>