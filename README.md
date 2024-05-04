# React Life Cycle Vis

💖 Reproducing [react lifecycle chart](https://projects.wojtekmaj.pl/react-lifecycle-methods-diagram/) with less than 200 lines (mermaid) markdown.

🤔 Plan to add more stuffs to make it more complete.

```mermaid
%%{
    init: {
        'theme': 'dark'
    }
}%%
block-beta
    classDef HIDDEN display:none;
    classDef BORDER_NONE fill:none, stroke:none;
    classDef DASH_LINE stroke-dasharray: 5,5, height:1px, stroke-width:1px;
    columns 10

%% row 0
DL_ROW_SUBROW_0[" "]:10
class DL_ROW_SUBROW_0 HIDDEN

%% row 1
    space:1

    Mounting["<h3>Mounting</h3>"]:3
    class Mounting BORDER_NONE

    Updating["<h3>Updating</h3>"]:3
    class Updating BORDER_NONE

    Unmounting["<h3>Unmounting</h3>"]:3
    class Unmounting BORDER_NONE

%% row 2
    block:D_ROW_2:10
        DL_ROW_2[" "]
        class DL_ROW_2 DASH_LINE
    end
    class D_ROW_2 BORDER_NONE

%% row 3
    space:1

    constructorCall["🔗 <b><a href="https://legacy.reactjs.org/docs/react-component.html#constructor" style="text-decoration:none;color:#ccc;">constructor()</a></b>"]:3

    NewProps["<i>New Props</i>"]
    class NewProps BORDER_NONE

    setStateCall["setState()"]
    class setStateCall BORDER_NONE

    forceUpdateCall["forceUpdate()"]
    class forceUpdateCall BORDER_NONE

    space:3

%% row 4
    space:1

    A_ROW_4_COL_2_4 <[" "]>(down):3
    A_ROW_4_COL_4_5 <[" "]>(down):1
    A_ROW_4_COL_5_6 <[" "]>(down):1
    A_ROW_4_COL_6_7 <[" "]>(down):1

    A_ROW_4_COL_8_10 <[" "]>(down):3

%% row 5
    renderPhase["<h3>Render\nPhase</h3>"]:1
    class renderPhase BORDER_NONE

    getDerivedStateFromPropsCall["<a href="https://legacy.reactjs.org/docs/react-component.html#static-getderivedstatefromprops" style="text-decoration:none;color:#ccc;">🔗 getDerivedState\nFromProps()</a>"]:6

    A_ROW_5_COL_8_10 <[" "]>(down):3

%% row 6
    space:1

    A_ROW_6_COL_2_4 <[" "]>(down):3

    A_ROW_6_COL_5_6 <[" "]>(down):1
    A_ROW_6_COL_6_7 <[" "]>(down):1
    A_ROW_6_COL_7_8 <[" "]>(down):1

    A_ROW_6_COL_8_10 <[" "]>(down):3

%% row 7
    space:1

    A_ROW_7_COL_2_4 <[" "]>(down):3

    shouldComponentUpdateCall["<a href="https://legacy.reactjs.org/docs/react-component.html#shouldcomponentupdate" style="text-decoration:none;color:#ccc;">🔗 should\nComponent\nUpdate()</a>"]:2
    A_ROW_7_COL_6_7 <[" "]>(down):1

    A_ROW_7_COL_8_10 <[" "]>(down):3

%% row 8
    space:1

    A_ROW_8_COL_2_4 <[" "]>(down):3
    A_ROW_8_COL_4_5<[" "]>(down):2
    class b8 BORDER_NONE

    A_ROW_8_COL_7_8 <[" "]>(down):1

    A_ROW_8_COL_8_10 <[" "]>(down):3

%% row 9
    space:1

    renderCall["🔗 <b><a href="https://legacy.reactjs.org/docs/react-component.html#render" style="text-decoration:none;color:#ccc;">render()</a></b>"]:6

    A_ROW_9_COL_8_10 <[" "]>(down):3

%% row 10
    block:D_ROW_10:10
        columns 1
        DL_ROW_10_SUBROW_1[" "]
        DL_ROW_10_SUBROW_2[" "]
        DL_ROW_10_SUBROW_3[" "]
        DL_ROW_10_SUBROW_4[" "]

        class DL_ROW_10_SUBROW_1,DL_ROW_10_SUBROW_2,DL_ROW_10_SUBROW_3 HIDDEN
        class DL_ROW_10_SUBROW_4 DASH_LINE
    end
    class D_ROW_10 BORDER_NONE

%% row 11
    space:1

    A_ROW_11_COL_2_4 <[" "]>(down):3

    A_ROW_11_COL_5_7 <[" "]>(down):3

    A_ROW_11_COL_8_10 <[" "]>(down):3

%% row 12
    preCommitPhase["<h3>Pre-commit\nPhase</h3>"]:1
    class preCommitPhase BORDER_NONE

    A_ROW_12_COL_2_4 <[" "]>(down):3

    getSnapshotBeforeUpdateCall["<a href="https://legacy.reactjs.org/docs/react-component.html#getsnapshotbeforeupdate" style="text-decoration:none;color:#ccc;">🔗 getSnapshot\nBeforeUpdate()</a>"]:3

    A_ROW_12_COL_8_10 <[" "]>(down):3

%% row 13
    block:D_ROW_13:10
        columns 1
        DL_ROW_13_SUBROW_1[" "]
        DL_ROW_13_SUBROW_2[" "]
        DL_ROW_13_SUBROW_3[" "]
        DL_ROW_13_SUBROW_4[" "]

        class DL_ROW_13_SUBROW_1,DL_ROW_13_SUBROW_2,DL_ROW_13_SUBROW_3 HIDDEN
        class DL_ROW_13_SUBROW_4 DASH_LINE
    end
    class D_ROW_13 BORDER_NONE

%% row 14
    space:1

    A_ROW_14_COL_2_4 <[" "]>(down):3

    A_ROW_14_COL_5_7 <[" "]>(down):3

    A_ROW_14_COL_8_10 <[" "]>(down):3

%% row 15
    commitPhase["<h3>Commit\nPhase</h3>"]:1
    class commitPhase BORDER_NONE

    reactUpdateDomAndRef["React update\nDoms and refs"]:6

    A_ROW_15_COL_8_10 <[" "]>(down):3

%% row 16
    space:1

    A_ROW_16_COL_2_4  <[" "]>(down):3
    A_ROW_16_COL_5_7  <[" "]>(down):3
    A_ROW_16_COL_8_10 <[" "]>(down):3

%% row 17
    space:1

    componentDidMountCall["🔗 <b><a href="https://legacy.reactjs.org/docs/react-component.html#componentdidmount" style="text-decoration:none;color:#ccc;">component\nDidMount()</a></b>"]:3
    componentDidUpdateCall["🔗 <b><a href="https://legacy.reactjs.org/docs/react-component.html#componentdidupdate" style="text-decoration:none;color:#ccc;">component\nDidUpdate()</a></b>"]:3
    componentWillUnmountCall["🔗 <b><a href="https://legacy.reactjs.org/docs/react-component.html#componentwillunmount" style="text-decoration:none;color:#ccc;">component\nWillUnmount()</a></b>"]:3

%% row inf
DL_ROW_INF_SUBROW_1[" "]:10
DL_ROW_INF_SUBROW_2[" "]:10
DL_ROW_INF_SUBROW_3[" "]:10
class DL_ROW_INF_SUBROW_1,DL_ROW_INF_SUBROW_2,DL_ROW_INF_SUBROW_3 HIDDEN

```
