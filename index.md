---
layout: page
title: The Missing Semester of Your CS Education (โครงการแปลภาษาไทย)
nositetitle: true
---

การเรียนในชั้นเรียนทำให้ผู้เรียนได้รับความรู้ด้านวิทยาการคอมพิวเตอร์มากมาย ไม่ว่าจะเป็น
ระบบปฏิบัติการ (operating systems) หรือการเรียนรู้โดยเครื่องจักร (machine learning)
แต่ยังมีหัวข้อหนึ่งที่ไม่ค่อยมีการกล่าวถึง และผู้เรียนมักถูกทิ้งให้ศึกษากันเอาเอง
หัวข้อนั้นก็คือการใช้เครื่องมืออย่างเชี่ยวชาญ ในกิจกรรมการเรียนนี้
เราจะสอนให้ผู้เรียนใช้การพิมพ์คำสั่งสู่ระบบปฏิบัติการด้วย command line ได้อย่างเชี่ยวชาญ
สามารถใช้โปรแกรมแก้ไขข้อความ (text editor) สามารถจัดการเวอร์ชันของงานที่ทำด้วย
version control systems ตลอดจนหัวข้ออื่นๆ

ผู้เรียนต้องฝึกฝนทักษะการใช้เครื่องมือเหล่านี้เป็นเวลาหลายร้อยชั่วโมง
และในชีวิตการทำงานจริงก็ใช้เวลาเป็นพันชั่วโมง ดังนั้น เราจึงคิดว่าการทำให้
การสอนทักษะเหล่านี้เป็นไปได้ง่ายและสบายที่สุดเป็นสิ่งสำคัญ การใช้เครื่องมือ
เหล่านี้ให้เชี่ยวชาญทำให้ท่านใช้เวลาศึกษาเอาเองน้อยลง และยังสามารถ
แก้ปัญหาที่อาจยากเกินขอบเขตเดิมของท่านได้ด้วย

[ศึกษาแรงจูงใจที่ทำให้เกิดวิชานี้](/about/)

{% comment %}

Classes teach you all about advanced topics within CS, from operating systems
to machine learning, but there’s one critical subject that’s rarely covered,
and is instead left to students to figure out on their own: proficiency with
their tools. We’ll teach you how to master the command-line, use a powerful
text editor, use fancy features of version control systems, and much more!

Students spend hundreds of hours using these tools over the course of their
education (and thousands over their career), so it makes sense to make the
experience as fluid and frictionless as possible. Mastering these tools not
only enables you to spend less time on figuring out how to bend your tools to
your will, but it also lets you solve problems that would previously seem
impossibly complex.

Read about the [motivation behind this class](/about/).
{% endcomment %}

{% comment %}
# Registration

Sign up for the IAP 2020 class by filling out this [registration form](https://forms.gle/TD1KnwCSV52qexVt9).
{% endcomment %}

# ตารางเรียน

{% comment %}
**Lecture**: 35-225, 2pm--3pm<br>
**Office hours**: 32-G9 lounge, 3pm--4pm (every day, right after lecture)
{% endcomment %}

<ul>
{% assign lectures = site['2020'] | sort: 'date' %}
{% for lecture in lectures %}
    {% if lecture.phony != true %}
        <li>
        <strong>{{ lecture.date | date: '%-m/%d/%y' }}</strong>:
        {% if lecture.ready %}
            <a href="{{ lecture.url }}">{{ lecture.title }}</a>
        {% else %}
            {{ lecture.title }} {% if lecture.noclass %}[no class]{% endif %}
        {% endif %}
        </li>
    {% endif %}
{% endfor %}
</ul>

Video recordings of the lectures are available [on
YouTube](https://www.youtube.com/playlist?list=PLyzOVJj3bHQuloKGG59rS43e29ro7I57J).

# เกี่ยวกับรายวิชานี้

**ผู้สอน**: ผู้สอนเดิมของวิชานี้ประกอบด้วย [Anish](https://www.anishathalye.com/), [Jon](https://thesquareplanet.com/), and [Jose](http://josejg.com/).<br>
**สอบถาม**: ติดต่อทางอีเมล์ได้ที่ [missing-semester@mit.edu](mailto:missing-semester@mit.edu).

TN: กรณีสอบถามเกี่ยวกับการแปล และคำถามที่จะถามทีมแปลภาษาไทย ให้ติดต่อที่
[ห้องปฏิบัติการวิจัยการประมวลผลสมรรถนะสูงและเครือข่าย มหาวิทยาลัยเกษตรศาสตร์](https://hpcnc.in.th) 
สำหรับโครงการสอนสดของห้องปฏิบัติการ นิสิตปัจจุบัน มหาวิทยาลัยเกษตรศาสตร์ 
ให้ติดต่อที่ห้องปฏิบัติการ ห้อง 801 อาคารภาควิชาวิศวกรรมคอมพิวเตอร์ มหาวิทยาลัยเกษตรศาสตร์ 
(บุคคลภายนอกให้ติดต่อทางช่องทางที่กำหนดเท่านั้น)

# การเผยแพร่นอก MIT

คณะผู้สอนได้นำชั้นเรียนนี้ไปถ่ายนอดให้นอก MIT เพื่อแบ่งปันความรู้ โดยสามารถ
ศึกษาข้อมูลเพิ่มเติมได้จากแหล่งที่ให้นี้

 - [Hacker News](https://news.ycombinator.com/item?id=22226380)
 - [Lobsters](https://lobste.rs/s/ti1k98/missing_semester_your_cs_education_mit)
 - [/r/learnprogramming](https://www.reddit.com/r/learnprogramming/comments/eyagda/the_missing_semester_of_your_cs_education_mit/)
 - [/r/programming](https://www.reddit.com/r/programming/comments/eyagcd/the_missing_semester_of_your_cs_education_mit/)
 - [Twitter](https://twitter.com/jonhoo/status/1224383452591509507)
 - [YouTube](https://www.youtube.com/playlist?list=PLyzOVJj3bHQuloKGG59rS43e29ro7I57J)

{% comment %}
Some more URLs:

- https://news.ycombinator.com/item?id=27154577
- https://news.ycombinator.com/item?id=34934216
- https://www.reddit.com/r/learnprogramming/comments/nca1v3/mit_the_missing_semester_of_your_cs_education/
- https://www.reddit.com/r/compsci/comments/eyywv8/the_missing_semester_of_your_cs_education_from_mit/
- https://www.reddit.com/r/programming/comments/io7nq3/the_missing_semester_of_your_cs_education_mit/
- https://twitter.com/MIT_CSAIL/status/1349766980413263873
- https://twitter.com/MIT_CSAIL/status/1481676163491659780
- https://twitter.com/MIT_CSAIL/status/1581313961093484545
{% endcomment %}

# Translations

- [Chinese (Simplified)](https://missing-semester-cn.github.io/)
- [Chinese (Traditional)](https://missing-semester-zh-hant.github.io/)
- [Japanese](https://missing-semester-jp.github.io/)
- [Korean](https://missing-semester-kr.github.io/)
- [Portuguese](https://missing-semester-pt.github.io/)
- [Russian](https://missing-semester-rus.github.io/)
- [Serbian](https://netboxify.com/missing-semester/)
- [Spanish](https://missing-semester-esp.github.io/)
- [Turkish](https://missing-semester-tr.github.io/)
- [Vietnamese](https://missing-semester-vn.github.io/)
- [Arabic](https://missing-semester-ar.github.io/)
- [Italian](https://missing-semester-it.github.io/)
- [Persian](https://missing-semester-fa.github.io/)
- [German](https://missing-semester-de.github.io/)
- [Bengali](https://missing-semester-bn.github.io/)

โปรดทราบว่า ข้อมูลข้างต้นเป็นลิงค์ไปยังการแปลโดยผู้แปลอิสระ ทางคณะผู้สอน
ไม่ได้ตรวจสอบความถูกต้อง

Have you created a translation of the course notes from this class? Submit a
[pull request](https://github.com/missing-semester/missing-semester/pulls) so
we can add it to the list!

## Acknowledgements

We thank Elaine Mello, Jim Cain, and [MIT Open
Learning](https://openlearning.mit.edu/) for making it possible for us to
record lecture videos; Anthony Zolnik and [MIT
AeroAstro](https://aeroastro.mit.edu/) for A/V equipment; and Brandi Adams and
[MIT EECS](https://www.eecs.mit.edu/) for supporting this class.

---

<div class="small center">
<p><a href="https://github.com/missing-semester/missing-semester">Source Code (ฉบับเดิมภาษาอังกฤษ / English Original)</a> / <a href="https://github.com/LunaticNeko/missing-semester-th">Source Code (โครงการแปลภาษาไทย / Thai Translation Project)</a></p>
<p>Licensed under CC BY-NC-SA. (Thai Translation Project also CC BY-NC-SA.)</p>
<p>See <a href="/license/">here</a> for contribution &amp; translation guidelines.</p>
</div>
