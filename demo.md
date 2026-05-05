---
marp: true
theme: dunwoody
paginate: true
---

<!-- header: Dunwoody Marp Theme-->

<!-- _class: lead -->

# Towards a Unified Dunwoody Presentation Theme

#### Let's graduate from other slides!

<br>

**Author: Joshua Luppes**
Dunwoody College of Technology
YYYY/MM/DD

---

<!-- _header: Table of Contents -->

1. Introduction
1. Code Blocks
1. Mathematical Formulas
1. Figures

---

<!-- _header: Introduction -->

- Marp is software for creating **slides** using **Markdown**.
  - Basic Markdown syntax is supported.
- You can move to the next page simply by inserting a horizontal rule `---` in Markdown.$^1$

> 1: Since Marp is developed according to the CommonMark Markdown specification, the "footnote" syntax (the one using `[^1]`), which is not part of CommonMark, is not provided. Therefore, I implemented a pseudo-footnote by referring to https://github.com/marp-team/marp/discussions/150#discussioncomment-1302384.

---

<!-- _header: Code Blocks -->

```javascript
console.log("Testing!");
```

You can write code blocks like this.

```python
@app.route('/members/view/<int:id>')
def view_member(id):
    member = Members.query.get_or_404(id)
    memberships = Memberships.query.all()
    return render_template('view_member.html', member=member, memberships=memberships)
```

The width is automatically adjusted (refer to [Auto-scaling](https://github.com/marp-team/marp-core#auto-scaling-features) in the documentation).

---

<!-- _header: Mathemetical Formulas -->

$$ I\_{xx}=\int\int_Ry^2f(x,y)\cdot{}dydx $$

$$
f(x) = \int_{-\infty}^\infty
    \hat f(\xi)\,e^{2 \pi i \xi x}
    \,d\xi
$$

You can write mathematical formulas like this. Of course, inline $\LaTeX$ is also available.
You can also use emojis: :smile:

---

<!-- _header: Figures -->

1. First, download the image (`kenkyu_woman_seikou.png`) from [this Irasutoya link](https://www.irasutoya.com/2018/10/blog-post_723.html) by right-clicking.
2. Create a directory named `images` in the same directory as this Markdown file, and place the downloaded image there. Now you're all set.

![w:300 center](./images/kenkyu_woman_seikou.png)
